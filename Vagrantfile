# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|  
  config.vm.define "dockerVM1" do |dockerVM1|
    dockerVM1.vm.box = "ubuntu/xenial64"
    dockerVM1.vm.provision "docker"
    dockerVM1.vm.hostname  = "dockerVM1"
    dockerVM1.vm.synced_folder ".", "/Docker Swarm"
    dockerVM1.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
    end
  end

  config.vm.define "dockerVM2" do |dockerVM2|
    dockerVM2.vm.box = "ubuntu/xenial64"
    dockerVM2.vm.provision "docker"
    dockerVM2.vm.hostname  = "dockerVM2"
    dockerVM2.vm.synced_folder ".", "/Docker Swarm"
    dockerVM2.vm.provider "virtualbox" do |vb|
        vb.memory = "1024"
    end
  end
end
