This repository provides Vagrantfile with ubuntu/trusty64 box to install and setup wordpress

## Usage

For more information about Vagrant usage, see Vagrant's documentation

   1 - Download Vagrantfile to a directory, navigate to inside the directory

   2 - Download the setup shell script, the Vagrantfile needs it to install and setup Apache,Mysql,Ssh,Wordpress...

   3 - Run the box with a single comande -> vagrant up.
    
```  
$ vagrant up
Bringing machine 'default' up with 'virtualbox' provider...
==> default: Importing base box 'ubuntu/trusty64'...
==> default: Matching MAC address for NAT networking...
==> default: Checking if box 'ubuntu/trusty64' version '20190514.0.0' is up to date...
==> default: Setting the name of the VM: lab-vm
==> default: Clearing any previously set forwarded ports...
==> default: Clearing any previously set network interfaces...
==> default: Preparing network interfaces based on configuration...
    default: Adapter 1: nat
    default: Adapter 2: hostonly
==> default: Forwarding ports...
    default: 80 (guest) => 8080 (host) (adapter 1)
    default: 22 (guest) => 2222 (host) (adapter 1)
==> default: Running 'pre-boot' VM customizations...
```

4 - in your browser localhost:8080/wp-admin/install.php

<img src="https://github.com/SoufiyanAk/Vagrant-wordpress-ubuntu/blob/main/home.png?raw=true" width="1000" height="400">

5 - To SSH into the box, use vagrant ssh.

6 - To destroy the box, use vagrant destroy.

