# VirtualBox Installation

This directory contains screenshots walking you through the creation of Linux virtual machine (or VM) under VirtualBox.

VirtualBox is a free VM manager program that is well supported under Windows, OSX, and Linux. It can be downloaded here:

https://www.virtualbox.org/wiki/Downloads

If you don't have a specific distribution of Linux you prefer using, we recommend Ubuntu server. Download the latest LTS or long term support version. Since we're focusing on a server application, the desktop version of Ubuntu isn't really needed - we're not using a GUI. Ubuntu may be downloaded from:

http://www.ubuntu.com/download/server

### Download [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
![VirtualBox1](/VMinstall/virtualbox1.png?raw=true)

### Download [Ubuntu server LTS](http://www.ubuntu.com/download/server)
![VirtualBox2](/VMinstall/virtualbox2.png?raw=true)

#### Launch VirtualBox, create a new VM by selecting the blue 'New' icon. Select the 'Linux' OS type and 'Ubuntu (64-bit)' Version.
![VirtualBox3](/VMinstall/virtualbox3.png?raw=true)

### Select at least '768' megabytes of allocated memory or RAM
![VirtualBox4](/VMinstall/virtualbox4.png?raw=true)

### The default '8' gigabytes of disk space is sufficient
![VirtualBox5](/VMinstall/virtualbox5.png?raw=true)

### Any of hard disk file types are acceptable, the default 'VDI' or VirtualBox Disk Image is fine
![VirtualBox6](/VMinstall/virtualbox6.png?raw=true)

### Select 'Dynamically allocated' hard drive
![VirtualBox7](/VMinstall/virtualbox7.png?raw=true)

### Select an appropriate location to store this VM on your host
![VirtualBox8](/VMinstall/virtualbox8.png?raw=true)

### Select the Ubuntu ISO image that you downloaded prior, this will be utilizied upon the initial first boot of your VM host
![VirtualBox9](/VMinstall/virtualbox9.png?raw=true)

### Once Ubuntu boots, select an appropreiate language - we assume English, this is pre-selected - just press enter when this selection is presented
![VirtualBox10](/VMinstall/virtualbox10.png?raw=true)

### Press enter to select 'Install Ubuntu Server'
![VirtualBox11](/VMinstall/virtualbox11.png?raw=true)

### Select a language, again we assume English - press enter for this default selection
![VirtualBox12](/VMinstall/virtualbox12.png?raw=true)

### Select a location, the default is 'United States' - press enter for this default selection. The default
![VirtualBox13](/VMinstall/virtualbox13.png?raw=true)

### No keyboard detection is required, the default 'No'
![VirtualBox14](/VMinstall/virtualbox14.png?raw=true)

### Select the default 'English (US)' .. this assumes you're using a US English keyboard layout
![VirtualBox15](/VMinstall/virtualbox15.png?raw=true)

### Choose a VM hostname, the default 'ubuntu' is fine or choosen your own
![VirtualBox16](/VMinstall/virtualbox16.png?raw=true)

### Create an account on the VM, this field is free form.
![VirtualBox17](/VMinstall/virtualbox17.png?raw=true)

### Select a username, no spaces allowed or special control characters are allow here
![VirtualBox18](/VMinstall/virtualbox18.png?raw=true)

### Enter in a password, the next screen will request the same password again for verification
![VirtualBox19](/VMinstall/virtualbox19.png?raw=true)

### Select 'No' for home directory encryption, that's not within scope for this tutorial
![VirtualBox20](/VMinstall/virtualbox20.png?raw=true)

### Select the auto detected time zone or overwrite with your value
![VirtualBox21](/VMinstall/virtualbox21.png?raw=true)

### Select the default (by pressing enter), 'Guided - use entire disk and setup LVM' for disk partitions
![VirtualBox22](/VMinstall/virtualbox22.png?raw=true)

### Select the default (and likely only presented) virtual hard drive
![VirtualBox23](/VMinstall/virtualbox23.png?raw=true)

### Select the non-default 'Yes' to write changes to disk and configure LVM
![VirtualBox24](/VMinstall/virtualbox24.png?raw=true)

### Select the default volume group size
![VirtualBox25](/VMinstall/virtualbox25.png?raw=true)

### Select the non-default 'Yes' to write changes to disk
![VirtualBox26](/VMinstall/virtualbox26.png?raw=true)

### Leave the default proxy sertting blank. The installation takes several minutes to complete.
![VirtualBox27](/VMinstall/virtualbox27.png?raw=true)

### Select 'No automatic updates'
![VirtualBox28](/VMinstall/virtualbox28.png?raw=true)

### None of the software selection items are required, we recommend selecting the 'OpenSSH server' option
![VirtualBox29](/VMinstall/virtualbox29.png?raw=true)

### Select 'Yes' for the default Grub writen to MBR record
![VirtualBox30](/VMinstall/virtualbox30.png?raw=true)

### Select 'Continue' the default, which will complete the installation and present a login prompt
![VirtualBox31](/VMinstall/virtualbox31.png?raw=true)

### Login to the console with your specificed credentials
![VirtualBox32](/VMinstall/virtualbox32.png?raw=true)

### Download the archive for this tutorial with the following commands.
![VirtualBox33](/VMinstall/virtualbox33.png?raw=true)
```
wget -O tutorial.tgz https://github.com/0xreid/ansible-network-automation-tutorial/archive/master.tar.gz
tar xzf tutorial.tgz
cd nanog65-automation-tutorial-master
sudo apt-get install python-pip python-dev
sudo pip install -r requirements.txt
```
