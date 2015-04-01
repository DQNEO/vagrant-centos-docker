Vagrant.configure(2) do |config|

  config.vm.box = "chef/centos-7.0"

  config.vm.provision "shell", inline: <<-SHELL
    sudo yum -y update device-mapper
    sudo yum -y install docker
    sudo systemctl enable docker
    sudo systemctl start docker
    sudo docker pull busybox
    sudo docker run --rm  busybox echo hello world
  SHELL

end
