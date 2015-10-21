# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network :forwarded_port, host: 10080, guest: 80

  config.ssh.pty = true

  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get update
    sudo apt-get upgrade
  SHELL

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "vagrant.yml"
  end

end
