vagrant-devstack
================

Vagrantfile for setting up devstack.

Dependencies
==============
* Vagrant
* Virtualbox


Setup
==============

Just run:
``````sh
vagrant up
``````
This can take some time.

Usage
===================
The OpenStack webinterface can be accessed under: http:locahost/8080.

  - Username admin or demo
  - Password nova

You can access the CLI:
``````````````sh
vagrant ssh
cd devstack
source openrc demo demo
``````````````
Now you're able to access the OpenStack modules via the command line.
Examples:
````````````sh
#Get a list of running computing nodes
nova list
#Get the list of glance images
glance image-list
````````````
