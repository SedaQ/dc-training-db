# Run SedaQ Training Services in Docker Containers within Vagrant

* tested on **Linux** and **Mac**

## Prerequisities (Vagrant)

Install the following technology:

Technology | URL to Download                           | Version
---------- | ---------------                           | -------
VirtualBox | https://www.virtualbox.org/wiki/Downloads | 5.2.34+
Vagrant    | https://www.vagrantup.com/downloads.html  | 2.0.2+
Vagrant Disk Plugin | https://github.com/sprotheroe/vagrant-disksize | 0.1.3+

## Prerequisities (Inside the Vagrant Box)
The following requirements should be already satisfied by using Vagrant:

Technology        | URL to Download                  | Version
----------------- | ------------                     | ------------------
Docker            | https://docs.docker.com/install/ | 19.03.0+
Docker Compose    | https://docs.docker.com/compose/ | 1.25+

## Run Vagrant VM

* **8GB RAM are required for the VM**

1. Create and connect to virtual machine.

```shell
$ vagrant box update
$ vagrant up
$ vagrant ssh
```
    
2. Within the virtual machine, change current directory into `/vagrant`.

```shell
$ cd /vagrant
```
	
## Run the Services

```shell
$ docker-compose up
```
