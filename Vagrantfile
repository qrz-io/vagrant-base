# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "scotch/box"
  config.vm.network "private_network", ip: "192.168.10.10"
  config.vm.hostname = "qrz"
  config.vm.synced_folder ".", "/var/www", :nfs => { :mount_options => ["dmode=777","fmode=777"] }
  config.vm.provider "virtualbox" do |v|
          v.memory = 4096
          v.cpus = 8
      end
end
