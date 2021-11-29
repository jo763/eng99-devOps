# DevOps Intro
## Development Env
* Install Vagrant
## Linux Commands
* `vagrant up`
* `vagrant destroy`
* `vagrant reload`
* `systemctl status nginx`
* `vagrant ssh`

* ```
Vagrant.configure("2") do |config|
 # choose the os/box/distro
 config.vm.box = "ubuntu/xenial64"
 config.vm.network "private_network", ip: "192.168.10.100"
 # vagrant destroy
 # vagrant up
 # vagrant reload - quicker and same as destroy and up
end
```

 - Who am I `uname -a`
 - Where am I `pwd`
 - list dir or all `ls` or `ls -a`
 - copy file `cp filename destination`
 - cut or rename `mv filename destination`
 - create file `touch filename`
 - create folder `mkdir`
 - how to navigate `cd foldername` go up a folder `cd ..`
 - deleting file folders `rm -rf namefolder`

 **File Permissions**
 - Read `r`, Write `W` and executable `x`
 - How to check permissions `ll`
 - Change permission `chmod` permission `r` or `w` etc filename.
 - Find all processes running `top`
 - hot to kill a process `kill` ID 

## What is DevOps?
DevOps is the combination of development and operations with a focus of working together, sharing responsibilities, using infrastructure as code to lead to greater efficiency. They use the automation of the deployment pipeline as well as shorter product cycle times using continuous integration, delivery and deployment
