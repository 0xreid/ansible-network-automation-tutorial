# Ansible 101 Network Automation Tutorial
This repository holds materials for a Ansible network automation tutorial presented at [NANOG65](https://www.nanog.org/meetings/abstract?id=2678) and RIPE71. The assumed audience for this tutorial are IP network engineers with no or minimal programming or 'DevOps' experience. The tutorial was first presented at [NANOG65](https://www.nanog.org/meetings/nanog65/home) on October 6th, 2015 in Montreal, Québec, Canada.

### Authors
* [Bronwyn Lewis](http://bronwynlewis.com/) - [@bronwyn](https://twitter.com/bronwyn)
* [Matt Peterson](mailto:matt@peterson.org) - [@dorkmatt](https://twitter.com/dorkmatt)

## Prerequisites
For environment simplicity, we assume a stock Ubuntu LTS 14.04.3 server installation. It is highly encouraged to run a Linux host within a virtualization setup, such as VirtualBox, VMware Fusion, or other virtualization platforms. It is possible to run [Ansible](http://www.ansible.com/) under other Linux distributions or even other operating systems, such as Mac OSX or FreeBSD. The on-screen tutorial will be given from Mac OSX, but the Ansible commands remain the same.

Within your host OS, ```Python 2.7.10``` or greater must be installed (the Python 3.x releases are untested) along with ```pip``` (the Python packager management tool). For instructions on how to install the correct version of python and pip, as well as running Ansible on Windows, please see the following links:

* [Python on Linux](http://docs.python-guide.org/en/latest/starting/install/linux/)
* [Python on Mac OSX](http://docs.python-guide.org/en/latest/starting/install/osx/)
* [Installing PIP](https://pip.pypa.io/en/latest/installing.html)
* [Windows 10 & Ansible](https://www.jeffgeerling.com/blog/2017/using-ansible-through-windows-10s-subsystem-linux) or [Windows w/ Cygwin & Ansible](https://www.jeffgeerling.com/blog/running-ansible-within-windows)

## Installation
Follow the [VirtualBox and Ubuntu VM installation instructions ](/VMinstall/README.md)  which include screenshots and descriptions for the required steps.

If you have an existing Linux environment that you're comfortable managing, the main steps are:
```
wget -O tutorial.tgz https://github.com/bronwynlewis/nanog65-automation-tutorial/archive/master.tar.gz
tar xzf tutorial.tgz
cd nanog65-automation-tutorial-master
sudo apt-get install python-pip python-dev
sudo pip install -r requirements.txt
```

## Directories

### workspace

This directory is meant to be used as a workspace to follow along with the hands-on tutorial portion of the talk. You'll be creating directories and files from scratch, as well as moving and editing existing reference files.

### full_example

This directory contains a more complete finished example of the tutorial for reference. (WIP)

### hello_world

Basic role to learn to generate files and print "Hello world" to a text file.

### ipcalc_example

This directory contains some basic examples of the ```ipaddr()``` filter in action - both IPv4 and IPv6.
