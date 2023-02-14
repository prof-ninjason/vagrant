# Version: 1.0.0
Vagrant.configure("2") do |config|
  config.vm.synced_folder '.', '/vagrant', disabled: true
  config.ssh.username = 'vagrant'
  config.ssh.password = 'vagrant'

  config.vm.define "pfsense" do |pfsense|
    pfsense.vm.box = "prof-ninjason/pfsense"
    pfsense.vm.hostname = "pfsense"
 
    # pfsense.vm.network "private_network", type: "dhcp", virtualbox__intnet: true
    pfsense.vm.network "private_network", ip: '192.168.10.60', virtualbox__intnet: true
 
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

  config.vm.define "owasp" do |owasp|
    owasp.vm.box = "prof-ninjason/owasp"
    owasp.vm.hostname = "owasp"

    owasp.vm.network "private_network", type: "dhcp", virtualbox__intnet: true

    owasp.vm.provider "virtualbox" do |vb|
      vb.name = "owasp"
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

  config.vm.define "onion" do |onion|
    onion.vm.box = "prof-ninjason/onion"
    onion.vm.hostname = "onion"
 
    onion.vm.network "private_network", type: "dhcp", virtualbox__intnet: true
    onion.vm.network "private_network", type: "dhcp", virtualbox__intnet: true

    onion.vm.provider "virtualbox" do |vb|
      vb.name = "onion"
      vb.memory = "4096"
      vb.cpus = "2"
      vb.gui = true
    end
  end
end
