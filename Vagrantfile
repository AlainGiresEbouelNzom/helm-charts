# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define "minikube" do |minikube|
    minikube.vm.hostname = "minikube"
    minikube.vm.box = "bento/ubuntu-20.04"
    minikube.vm.network "private_network", ip: "10.10.0.1"
    minikube.vm.synced_folder ".", "/vagrant"
    minikube.vm.boot_timeout = 600
    minikube.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
      vb.cpus = "2"
    end
   
  end

end
