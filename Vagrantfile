# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|

  config.vm.box = "puppetlabs/centos-7.0-64-nocm"
  config.ssh.insert_key = false # we use the insecure default key to simplify things

  config.vm.define "mybox" do |mybox|
    mybox.vm.network "private_network", ip: "192.168.33.10"
    mybox.vm.network "forwarded_port", guest: 8080, host: 8080
  end

end
