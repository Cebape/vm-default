# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.network "public_network", ip:"10.10.125.50", bridged:"ens160"
  config.vm.synced_folder "./sync_folder_host", "/home/vagrant/sync_folder_work", create: true
 
  # Configure boot timeout
  config.vm.boot_timeout=1600

  config.vm.provider "virtualbox" do |vb|
    # Display the VirtualBox GUI when booting the machine
    vb.gui = false
    # Customize the amount of memory on the VM:
    vb.memory = "1024"
  
    # vbox name
    vb.name = "vm-default"
  end
end