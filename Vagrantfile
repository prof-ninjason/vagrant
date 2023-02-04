# Version: 0.1.0
Vagrant.configure("2") do |config|
  config.vm.synced_folder '.', '/vagrant', disabled: true
  
  config.vm.box = "prof_ninjason/pfsense"
  config.vm.box_version = "0.1.0"
  
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.network "forwarded_port", guest: 443, host: 8443
  
  config.vm.network "private_network", type: "dhcp", virtualbox__intnet: true

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
  	vb.cpus = "2"
  end
end