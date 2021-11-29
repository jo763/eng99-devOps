# DevOps Intro
## Development Env
* Install Vagrant
## Linux Commands
- `vagrant up` Create virtual machine
- `vagrant destroy` Destroy virtual machine
- `vagrant reload` reload virtual machine
- `systemctl status nginx` - check the status of nginx
- `vagrant ssh` - connect to the virtual machine from bash

- Create Vagrantfile
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
 - deleting file + folders `rm -rf namefolder`
 - Display first 2 lines of a file `head -2 <filename>`
 - Display last 2 lines of a file `tail -2 <filename>`

 * File Permissions
 - Read `r`, Write `w` and executable `x`
 - How to check permissions `ll`
 - Change permission `chmod` permission `r` or `w` etc filename.
 - Find all processes running `top`
 - hot to kill a process `kill` ID


 ### Automate everything we have done manually
 - Automate everything we have done manually
 - install nginx and load it in the browser

### Startup Script
 - Simple startup bash script to update, upgrade packages and then install nginx: provisions.sh
 ```
!/bin/bash
sudo apt-get update -y
sudo apt-get upgrade -y
sudo apt-get install ngin-y
 ```
 - The script permission will need to be changed to executable via `chmod +x <filename>`

## Piping
- Allows standard output of one command to be used as the standard input of another command
- `command_1 | command_2 | command_3 | .... | command_N `


# DevOps
## What is DevOps?
 - DevOps is the combination of development and operations with a focus of working together, sharing responsibilities, using infrastructure as code to lead to greater efficiency. They use the automation of the deployment pipeline as well as shorter product cycle times using continuous integration, delivery and deployment.

## Benefits
- GOOD FOR BUSINESS
- Speed
- Rapid delivery - increase frequency and pace of delivery releases
- Reliability, good quality, changes are tested, easy to scale
- Better security
- Improved collaboration between devs and ops
- More deployments and projects are more likely to succeed

## Challenges in new Software Development Life Cycle (SDLC)
- Ease of use
- Flexibility
- Robustness
- Cost

## DevOps Principles
- Customer-centric action
- End-to-end responsibility
- Continuous improvement
- Automate everything
- Work as one team
- Monitor and test everything
