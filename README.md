# NANOG65 - Ansible network automation tutorial
This repository holds materials for a [Ansible network automation tutorial](https://www.nanog.org/meetings/abstract?id=2678). The assumed audience for this tutorial assumes IP network engineers with minimal programming or 'DevOps' experience. The tutorial was initially presented at [NANOG65](https://www.nanog.org/meetings/nanog65/home) on October 6th, 2015 in Montreal, Québec, Canada.

### Authors
* [Bronwyn Lewis](http://bronwynlewis.com/) - [@bronwyn](https://twitter.com/bronwyn)
* [Matt Peterson](mailto:matt@peterson.org) - [@dorkmatt](https://twitter.com/dorkmatt)

## Prerequisites
For environment simplicity, we highly assume a stock Ubuntu LTS 14.04.3 server installation. It is highly encouraged to run such a Linux host within a virtualization setup, such as VirtualBox or. VMware ESX/Fusion. It is possible to run [Ansible](http://www.ansible.com/) under other Linux distributions or even other operating systems, such as Mac OSX or FreeBSD. The on-screen tutorial will be given from Mac OSX, but the Ansible commands remain the same.

Within your host OS, ```Python 2.7.10``` or greater must be installed (the Python 3.x releases are untested) along with the ```pip``` (the Python packager management tool). Instructions on how to install the correct version of python and pip, as well as running Ansible on Windows, please see the following links:

* [Python on Linux](http://docs.python-guide.org/en/latest/starting/install/linux/)
* [Python on Mac OSX](http://docs.python-guide.org/en/latest/starting/install/osx/)
* [Installing PIP](https://pip.pypa.io/en/latest/installing.html)
* [Windows & Ansible - PROCEED WITH CAUTION](https://servercheck.in/blog/running-ansible-within-windows)

## Installation
* Checkout this git repo
```git clone https://github.com/bronwynlewis/nanog65-automation-tutorial.git```
* _OR_ download an archive
```wget https://github.com/bronwynlewis/nanog65-automation-tutorial/archive/master.zip```

Prereq: python 2.7.10 and pip 1.5

To install ```ansible```, its dependencies, and the ```netaddr``` package (required to use the ```ipaddr()``` Jinja2 text filter for IP address calculation), run:

```sudo pip install -r requirements.txt```

##Directories

###VMinstall

This directory has a screenshot walkthrough of creating a VirtualBox VM, along with a basic README with links to VirtualBox and Ubuntu for creating a VM for this tutorial. (optional, but recommend)

###workspace

This directory is meant to be used as a workspace to follow along with the hands-on tutorial portion of the talk. You'll be creating directories and files from scratch.

###main_example

This directory contains a more complete finished example of the tutorial for reference. (WIP)

###ipcalc_example

This directory contains some examples of the ```ipaddr()``` filter in action - both IPv4 and IPv6. (WIP)
