# CraftCMS on Docker
This project is designed to create a series of Docker containers running CraftCMS. This process uses multiple containers instead of stuffing everything into one container. This makes the entire process more robust and extensible.

## Requirements
* [Ansible 2+](https://www.ansible.com/)
* [Vagrant 2+](https://www.vagrantup.com/)
* Vagrant Plugins:
  * vagrant-vbguest
* [VirtualBox 5+](https://www.virtualbox.org/)

## Get Started

### Setup .env file
Rename ```example_env``` to ```.env``` and set the values. The values are as follows:

* **MYSQL_ROOT_PASSWORD** - the root password for MySQL
* **MYSQL_USER** - the user your site will use
* **MYSQL_PASSWORD** - the password for the user
* **MYSQL_DATABASE** - the name of the database for your site
* **NEWUSER** - a username that will be created on the server
* **SSH_KEY** - the path to the SSH key for the created user

### Run
Run the script: ```/vagrant/.development_build.sh```
