Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.network "private_network", ip: "192.168.33.15"
  config.vm.provision "docker"
  # require vagrant plugin install vagrant-docker-compose
  # https://github.com/leighmcculloch/vagrant-docker-compose
  config.vm.provision :docker_compose
  config.vm.synced_folder ".", "/vagrant", disabled: true
end
