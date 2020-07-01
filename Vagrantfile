


Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-8"
  config.vm.hostname = "conda-apolo.test.lan"
  config.vm.network :private_network, ip: "192.168.2.0"

    config.vm.provider :virtualbox do |vb|
      vb.name = "conda"
      vb.memory = 1024
      vb.cpus = 2

      config.vm.provision :ansible do |ansible|
        ansible.inventory_path = "ansible/practice/inventory"
        ansible.verbose = 'vvv'
        ansible.playbook = "ansible/practice.yml"
        
    end
  end
