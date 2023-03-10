# Version: 1.1.1 
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
      vb.memory = "4096"
      vb.cpus = "2"
      vb.gui = true
    end
  end

  config.vm.define "ub1404" do |ub1404|
    # greenbone.vm.box = "prof-ninjason/greenbone"
    ub1404.vm.box = "rapid7/metasploitable3-ub1404"
    ub1404.vm.hostname = "ub1404"

    ub1404.vm.network "private_network", type: "dhcp", virtualbox__intnet: true

    ub1404.vm.provider "virtualbox" do |vb|
      vb.name = "ub1404"
      vb.memory = "2048"
      vb.cpus = "2"
      vb.gui = true
    end
  end
  
  config.vm.define "greenbone" do |greenbone|
    greenbone.vm.box = "prof-ninjason/greenbone"
    greenbone.vm.hostname = "greenbone"

    greenbone.vm.network "private_network", type: "dhcp", virtualbox__intnet: true

    greenbone.vm.provider "virtualbox" do |vb|
      vb.name = "Greenbone"
      vb.memory = "4096"
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

  config.vm.define "win10" do |win10|
    win10.vm.box = "prof-ninjason/win10"
    win10.vm.box = "gusztavvargadr/windows-10"
    win10.vm.hostname = "win10"

    win10.vm.network "private_network", type: "dhcp", virtualbox__intnet: true

    win10.vm.provider "virtualbox" do |vb|
      vb.name = "Win10"
      vb.memory = "4096"
      vb.cpus = "2"
      vb.gui = true
    end
  end

  config.vm.define "win11" do |win11|
    win11.vm.box = "prof-ninjason/win11"
    win11.vm.hostname = "win11"

    win11.vm.network "private_network", type: "dhcp", virtualbox__intnet: true

    win11.vm.provider "virtualbox" do |vb|
      vb.name = "Win11"
      vb.memory = "4096"
      vb.cpus = "2"
      vb.gui = true
    end
  end

  config.vm.define "rhel8" do |rhel8|
    rhel8.vm.box = "prof-ninjason/rhel8"
    rhel8.vm.box = "generic/rhel8"
    rhel8.vm.hostname = "rhel8"

    rhel8.vm.network "private_network", type: "dhcp", virtualbox__intnet: true

    rhel8.vm.provider "virtualbox" do |vb|
      vb.name = "Rhel8"
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
