# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

  # boxes at https://atlas.hashicorp.com/search.
  config.vm.box = "ubuntu/xenial64"

  config.vm.box_check_update = false

  config.vm.network "forwarded_port", guest: 80, host: 80

  # Provision
  config.vm.provision "ansible" do |ansible|
    # ansible.verbose = "vvv"
    ansible.playbook = "playbook.yml"

  end
end
