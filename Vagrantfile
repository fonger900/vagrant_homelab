# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
    config.vm.define "ubuntu1" do |cfg|
      cfg.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
        vb.cpus = 1
        vb.name = "ubuntu1"
      end
      cfg.vm.box = "bento/ubuntu-18.04"
      cfg.vm.hostname = "ubuntu1"
      cfg.vm.network :private_network, ip: "192.168.38.105", gateway: "192.168.38.1", dns: "8.8.8.8"
      cfg.vm.network "forwarded_port", guest: 22, host: 5221
      cfg.disksize.size = '20GB'
    end
  
    config.vm.define "ubuntu2" do |cfg|
      cfg.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
        vb.cpus = 1
        vb.name = "ubuntu2"
      end
      cfg.vm.box = "bento/ubuntu-18.04"
      cfg.vm.hostname = "ubuntu2"
      cfg.vm.network :private_network, ip: "192.168.38.106", gateway: "192.168.38.1", dns: "8.8.8.8"
      cfg.vm.network "forwarded_port", guest: 22, host: 5222
      cfg.disksize.size = '20GB'
    end
  
    config.vm.define "ubuntu3" do |cfg|
      cfg.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
        vb.cpus = 1
        vb.name = "ubuntu3"
      end
      cfg.vm.box = "bento/ubuntu-18.04"
      cfg.vm.hostname = "ubuntu3"
      cfg.vm.network :private_network, ip: "192.168.38.107", gateway: "192.168.38.1", dns: "8.8.8.8"
      cfg.vm.network "forwarded_port", guest: 22, host: 5223
      cfg.disksize.size = '20GB'
    end
  end
  