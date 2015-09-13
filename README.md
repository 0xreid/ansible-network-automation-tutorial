# NANOG65 - Ansible network automation tutorial
Files for the network automation tutorial at NANOG65.

These installation instructions assume that you are using the [Ubuntu VirtualBox VM]() provided for this tutorial, or at least have python 2.7.10 and pip 7 installed on Mac OSX or Linux. For instructions on how to install the correct version of python and pip, as well as running Ansible on Windows, please see the following links:

[Python on Linux](http://docs.python-guide.org/en/latest/starting/install/linux/)
[Python on Mac OSX](http://docs.python-guide.org/en/latest/starting/install/osx/)
[Installing PIP](https://pip.pypa.io/en/latest/installing.html)

[Windows & Ansible - PROCEED WITH CAUTION](https://servercheck.in/blog/running-ansible-within-windows)

## Installation
Prereq: python 2.7.10 and pip 7

To install ```ansible```, its dependencies, and the ```netaddr``` package (required to use the ```ipaddr()``` Jinja2 filter for IP address calculation), run:

```sudo pip install -r requirements.txt```


