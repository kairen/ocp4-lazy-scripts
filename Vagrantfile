# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "generic/rhel8"
    config.vm.box_version = "3.2.4"
    config.vm.network "private_network", ip: "172.16.33.100"
  
    config.vm.provider "virtualbox" do |vb|
      vb.name = "ocp-builder"
      vb.memory = 4096
      vb.cpus = 2
    end
    config.vm.synced_folder "./", "/vagrant"
  end