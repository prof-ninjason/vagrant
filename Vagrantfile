# Version: 1.0.0
Vagrant.configure("2") do |config|
  config.vm.synced_folder '.', '/vagrant', disabled: true

  config.vm.define "pfsense" do |pfsense|
    pfsense.vm.box = "prof-ninjason/pfsense"
    pfsense.vm.hostname = "pfsense"
  
    # pfsense.ssh.username = 'vagrant'
    # pfsense.ssh.password = 'vagrant'
    
    pfsense.vm.network "private_network", type: "dhcp", virtualbox__intnet: true
  
    pfsense.vm.provider "virtualbox" do |vb|
      vb.name = "pfSense"
  	  vb.memory = "2048"
      vb.cpus = "2"
	  vb.gui = true
    end
  end

  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "prof-ninjason/ubuntu"
    ubuntu.vm.hostname = "ubuntu"
    
    ubuntu.vm.network "private_network", type: "dhcp", virtualbox__intnet: true
  
    ubuntu.vm.provider "virtualbox" do |vb|
      vb.name = "Ubuntu"
  	  vb.memory = "2048"
      vb.cpus = "2"
	  vb.gui = true
    end
  end

  config.vm.define "kali" do |kali|
    kali.vm.box = "prof-ninjason/kali"
    kali.vm.hostname = "kali"
    
    kali.vm.network "private_network", type: "dhcp", virtualbox__intnet: true
  
    kali.vm.provider "virtualbox" do |vb|
      vb.name = "Kali"
  	  vb.memory = "2048"
      vb.cpus = "2"
	  vb.gui = true
    end
  end
end
