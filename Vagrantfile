Vagrant.configure("2") do |config|
  config.vm.define "master" do |master|
    master.vm.box = "ubuntu/jammy64"
    master.vm.hostname = "master"
    master.vm.network "private_network", ip: "192.168.56.10"
    master.vm.provider "virtualbox" do |vb|
      vb.name = "master"
      vb.memory = "2048"
      vb.cpus = 2
    end
  end

  config.vm.define "slave" do |slave|
    slave.vm.box = "ubuntu/jammy64"
    slave.vm.hostname = "slave"
    slave.vm.network "private_network", ip: "192.168.56.11"
    slave.vm.provider "virtualbox" do |vb|
      vb.name = "slave"
      vb.memory = "2048"
      vb.cpus = 2
    end
  end

  config.vm.define "manager" do |manager|
    manager.vm.box = "ubuntu/jammy64"
    manager.vm.hostname = "manager"
    manager.vm.network "private_network", ip: "192.168.56.12"
    manager.vm.provider "virtualbox" do |vb|
      vb.name = "manager"
      vb.memory = "2048"
      vb.cpus = 2
    end
  end
end
