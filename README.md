# General
This repo is supposed to help set up new pc's.
The idea is: 

1. install Prerequesites on new pc
2. get repo folder on usb stick from another pc
3. stick usb stick into new pc and decide which script to run

# Prerequesites:

1. fedora operating system installed
2. create user
3. Internet Access\
    this is not automated since you shouldn't write any passwords into repositories
4. install ansible
    `sudo dnf install -y ansible`

# How to run the script

## Casual pc setup:
  
1. Open Terminal in ansible-work-pc-setup folder
2. run:\
    `sudo ansible-playbook casual_pc_setup.yml -i hosts.yml`

## Developer pc setup:
It is not nescessary to run the casual install first, it is included in the developper yaml script

1. Open Terminal in ansible-work-pc-setup folder
2. run:\
    `sudo ansible-playbook dev_pc_setup.yml -i hosts.yml`


