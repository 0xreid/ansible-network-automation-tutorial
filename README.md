# Ansible Network Automation Tutorial
This repository holds materials for an Ansible network automation tutorial presented at [NANOG65](https://www.nanog.org/meetings/abstract?id=2678), [RIPE71](https://ripe71.ripe.net/programme/meeting-plan/tutorials/#mon1), and [APRICOT2017](https://2017.apricot.net/program/schedule/#/day/9/network-automation-ansible-101). The assumed audience for this tutorial are IP network engineers with no or minimal programming or 'DevOps' experience. The tutorial was first presented at [NANOG65](https://www.nanog.org/meetings/nanog65/home) on October 6th, 2015 in Montreal, Québec, Canada.

### Authors
* [Bronwyn Lewis](http://bronwynlewis.com/) - [@bronwyn](https://twitter.com/bronwyn)
* [Matt Peterson](mailto:matt@peterson.org) - [@dorkmatt](https://twitter.com/dorkmatt)

## Prerequisites
For environment simplicity, we assume a stock Ubuntu LTS server installation. It is highly encouraged to run a Linux host within a virtualization setup, such as VirtualBox, VMware Fusion, or other virtualization platforms. It is possible to run [Ansible](http://www.ansible.com/) under other Linux distributions or even other operating systems, such as Mac OSX, FreeBSD, and Windows 10.

Within your host OS, ```Python 2.7.10``` or greater must be installed (the Python 3.x releases are untested) along with ```pip``` (the Python packager management tool). For instructions on how to install the correct version of python and pip, as well as running Ansible on Windows, please see the following links:

* [Python on Linux](http://docs.python-guide.org/en/latest/starting/install/linux/)
* [Python on Mac OSX](http://docs.python-guide.org/en/latest/starting/install/osx/)
* [Installing PIP](https://pip.pypa.io/en/latest/installing.html)
* [Windows 10 & Ansible](https://www.jeffgeerling.com/blog/2017/using-ansible-through-windows-10s-subsystem-linux) or [Windows w/ Cygwin & Ansible](https://www.jeffgeerling.com/blog/running-ansible-within-windows)

## Installation
Follow the [VirtualBox and Ubuntu VM installation instructions ](/VMinstall/README.md) which include screenshots and descriptions for the required steps (note: the screenshots show an older Ubuntu release and slightly different git repo name, however the general directions still apply).

If you have an existing Linux environment that you're comfortable managing, the main steps are:
```
wget -O tutorial.tgz https://github.com/bronwynlewis/ansible-network-automation-tutorial/archive/master.tar.gz
tar xzf tutorial.tgz
cd ansible-network-automation-tutorial-master
sudo apt-get install python-pip python-dev
sudo pip install -r requirements.txt
```
### failure to build cryptography

If, in the ```pip install -r requirements.txt``` step, the cryptography build and subsequently the package installation fails, then you should check if all the dependencies are met. Check out this Stack Overflow post on the subject: [Failed to install Python Cryptography package with PIP and setup.py](https://stackoverflow.com/questions/22073516/failed-to-install-python-cryptography-package-with-pip-and-setup-py)

## Directories

### ansible101

#### workspace

This directory is meant to be used as a workspace to follow along with the hands-on tutorial portion of the talk. You'll be creating directories and files from scratch, as well as moving and editing existing reference files.

#### hello_world

Basic role to learn to generate files and print "Hello world" to a text file.

#### full_example

This directory contains a more complete finished example of the tutorial for reference.

#### ipcalc_example

This directory contains some basic examples of the ```ipaddr()``` filter in action - both IPv4 and IPv6.

### ansible102

This directory contains more complex examples, geared as an Ansible 102 tutorial.

### presentation

Copies of the slide deck used when the tutorial is presented at conferences.

### VMinstall

Tutorial to walk through the installation of a VM for the tutorial.
