Creating development environment with Vagrant and Ansible
=====================================

This project aims to provide a development environment by installing dependencies for fast and automated way using the [Ansible](http://www.ansible.com/).

All works on the virtual machine Debian 64-bit

Download and install:
------------
1. [Vagrant 1.8.1](https://www.vagrantup.com/docs/installation/)
2. [VirtualBox 5:16](https://www.virtualbox.org/wiki/Downloads)
3. [Ansible 2.1.2](http://docs.ansible.com/ansible/intro_installation.html)


running
-------

Clone this project using the 'flag --recursive` to the sub-modules are also cloned, and access the fast_env directory:

`` 
git clone --recursive git@github.com: glautonvieira / fast_env
`` 

`` 
cd fast_env
`` 

To start the VM:

``
vagrant up
``

To perform the roles:

``
vagrant provision
``

After that, Vagrant will create a new VM, configure it, and ...

Done! You have a development environment set up for automated testing installed!


Ansible install the following packages:
* git
* Ruby 2.3.1
* PhantomJS
* NodeJS
* Rbenv
* Rubocop


## Updating vendor/vagrant-roles

If some changes were updated in submodule you need to run the following git command in your root directory:

```
git submodule update
```


VM configuration
----------------
To learn more about the VM configuration options, see the documents in [Vagrant](http://docs.vagrantup.com/v2/virtualbox/configuration.html)
# fast_env
