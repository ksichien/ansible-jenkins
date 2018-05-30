### Ansible Jenkins
This is a collection of Ansible playbooks I've written to automate the installation, configuration and maintenance of a Vagrant VM running Jenkins on Debian GNU/Linux.
The installation of Docker, NodeJS 8 LTS and Ruby 2.4.3 are also performed.

## Usage

- Install Virtualbox, Vagrant & Ansible
```
$ sudo apt install virtualbox vagrant ansible
```
- Install the vbguest plugin for Vagrant
```
$ vagrant plugin install vagrant-vbguest
```
- Start the Vagrant virtual machine, this may take some time
```
$ vagrant up
```
- Execute the vagrant.yml playbook with Ansible on the Vagrant machine
```
$ vagrant provision
```
- Go to https://10.20.20.20 in a web browser, accept the self-signed certificate and follow the Jenkins Setup Wizard's instructions.
