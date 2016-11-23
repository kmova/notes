#Notes
Commands to get the virtual box and vagrant installed on Ubuntu 16.x
```
sudo apt-get update
sudo apt-get install virtualbox
vboxmanage  --version
sudo apt-get install vagrant
vagrant  version
```

Beginners commands
```
sudo vagrant init
#modify the Vagrantfile 
sudo vagrant up
sudo vagrant status
sudo vagrant ssh 
#login into the new VM created. 
sudo vagrant halt
sudo vagrant destroy
```

#Reference
* [Installing Vagrant and Virtual Box] (https://www.olindata.com/blog/2014/07/installing-vagrant-and-virtual-box-ubuntu-1404-lts)
* [Vagrant docs] (https://www.vagrantup.com/docs/)
* [Bento boxes] (https://github.com/chef/bento)
