# NANOG65 - Ansible network automation tutorial
Files for the network automation tutorial at NANOG65.

These installation instructions assume you are running at least ```python 2.7.10``` and ```pip 7``` installed on Mac OSX or Linux. For simplicity, it is recommended that you use a Linux VM (such as Debian or Ubuntu, but whatever flavor of Linux you are comfortable with is suitable). There are several virtualization options, including VirtualBox and VMware Fusion.

The on-screen tutorial will be given from Mac OSX, but the Ansible commands remain the same.

Instructions on how to install the correct version of python and pip, as well as running Ansible on Windows, please see the following links:

* [Python on Linux](http://docs.python-guide.org/en/latest/starting/install/linux/)
* [Python on Mac OSX](http://docs.python-guide.org/en/latest/starting/install/osx/)
* [Installing PIP](https://pip.pypa.io/en/latest/installing.html)

[Windows & Ansible - PROCEED WITH CAUTION](https://servercheck.in/blog/running-ansible-within-windows)

## Installation
Prereq: python 2.7.10 and pip 7

To install ```ansible```, its dependencies, and the ```netaddr``` package (required to use the ```ipaddr()``` Jinja2 filter for IP address calculation), run:

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
