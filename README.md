# DESCRIPTION

Vagrantfile to use Docker on CentOS 7

# USAGE

```
git clone https://github.com/DQNEO/vagrant-centos-docker.git
cd vagrant-centos-docker
vagrant up
vagrant ssh
```

After entering the vagrant machine

```
sudo docker pull busybox
sudo docker run --rm  busybox echo hello world
```
