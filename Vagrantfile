# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.ssh.insert_key = false

  config.vm.define "archlinux1201" do |archlinux1201|
    archlinux1201.vm.box="snowflake/archlinux"
    archlinux1201.vm.hostname = "archlinux64"
    
    archlinux1201.vm.network "private_network",
       ip:"172.24.0.3", 
       netmask:"255.255.255.0"

       #ADD MORE VIDEO MEMORY IF NEEDED (1-256MB max)
       archlinux1201.vm.provider "virtualbox" do |vb|
       vb.customize ["modifyvm", :id, "--vram", "256"]
    end
  end
end
