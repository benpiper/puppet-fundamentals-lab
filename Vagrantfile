# -*- mode: ruby -*-
# vi: set ft=ruby :

# See README.md for details

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "centos65-base"

  config.vm.define "puppetmaster" do |puppetmaster|
  
    puppetmaster.vm.hostname = "puppetmaster"
  
    puppetmaster.vm.network "private_network", ip: "172.31.0.201"
  
  end
  
  config.vm.define "wiki" do |wiki|
  
    wiki.vm.hostname = "wiki"
  
    wiki.vm.network "private_network", ip: "172.31.0.202"
  
  end
  
  config.vm.box = "ubuntu/trusty64"
  
  config.vm.define "wikitest" do |wikitest|
  
    wikitest.vm.hostname = "wikitest"
	
	wikitest.vm.network "private_network", ip: "172.31.0.203"

  end
  
end
