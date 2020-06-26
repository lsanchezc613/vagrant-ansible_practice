

Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-8"
  config.vm.hostname = "conda-apolo.test.lan"
  config.vm.network :private_network, ip: ""

    config.vm.provider :virtualbox do |vb|
      vb.name = "conda"
      vb.memory = 1024
      vb.cpus = 2
      
    end
  end
