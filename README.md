# NANOG65 - Ansible network automation tutorial
Files for the network automation tutorial at NANOG65.

These installation instructions assume you are running at least ```python 2.7.10``` and ```pip 7``` installed on Mac OSX or Linux. For simplicity, it is recommended that you use a Linux VM. There are several virtualization options, including VirtualBox and VMware Fusion.

Instructions on how to install the correct version of python and pip, as well as running Ansible on Windows, please see the following links:

[Python on Linux](http://docs.python-guide.org/en/latest/starting/install/linux/)
[Python on Mac OSX](http://docs.python-guide.org/en/latest/starting/install/osx/)
[Installing PIP](https://pip.pypa.io/en/latest/installing.html)

[Windows & Ansible - PROCEED WITH CAUTION](https://servercheck.in/blog/running-ansible-within-windows)

## Installation
Prereq: python 2.7.10 and pip 7

To install ```ansible```, its dependencies, and the ```netaddr``` package (required to use the ```ipaddr()``` Jinja2 filter for IP address calculation), run:

```sudo pip install -r requirements.txt```

##Directories

###main_example

###ipcalc_example

