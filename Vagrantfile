# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|  
  config.vm.define "dockerVM" do |dockerVM|
    dockerVM.vm.box = "ubuntu/xenial64"
    dockerVM.vm.network "private_network", ip: "192.168.33.50"
    dockerVM.vm.provision "docker"
    dockerVM.vm.hostname "dockerVM"
    dockerVM.vm.synced_folder ".", "/Docker Swarm"
    dockerVM.vm.provider "virtualbox" do |vb|
        vb.memory = "2048"
    end
  end
end
