# Ansible script to setup RaspberryPie from scratch

This repo is created to facilitate deployment of the following components
to a raspberry pie:

- packages : required debian packages for all other components
- samba: Deployment of samba + mounting usb disks and sshfs mountpoints
- transmission
- lansetup: Giving a static ip address to a lan
- apache: Deployment of Apache and creating the required virtual sites
- dotfiles: Deployment and installation of existme/MyDotFiles


To run ansible with your secret vault issue:
~~~shell
ansible-playbook --extra-vars "@secret.yml" -v main.yml 
~~~
