# -*- mode: ruby -*-
# vi: set ft=ruby :

# Usage Hints:
# 'vagrant up' will run provisioning on first boot.
# 'vagrant provision' will run provisioning scripts without rebuilding.

Vagrant.configure(2) do |config|

  config.vm.box = "debian/jessie64"

  config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = 'vagrant.yml'
    ansible.verbose = 'vvvv'
    ansible.sudo = true
  end

end
