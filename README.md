vagrant-centos64
================

A Vagrant kickstart file to provide the base necessities to create a personalized, vagrant basebox.

The VM's aren't guaranteed to be fully compliant, but this covers enough to enable me to build a base box, where I know the history of the base box. 

Purpose
-------

* A fast way to kickstart a CentOS base box. 
* Learning Vagrant, build base boxes

Usage
=====
HTTP approach

* Copy CentOS64.cfg to a webserver that will be accessible to the VM (keep in mind you need to be using NAT)
* Build the base box in VirtualBox (see source links for details)
* On the OS boot screen hit tab to get the OS options and enter:
 
``` 
ks https://raw.github.com/robbanfield/vagrant-centos64/master/CentOS64.cfg 
```
* Get your favourite caffeinated beverage
* Perform manual steps


Manual steps you need to do
---------------------------
* Install the VBoxLinuxAdditions
* Update UseDNS to no in /etc/ssh/sshd_config (Optional - depends on your use case)

Gotchas
=======
* Assumes Disk 1 of Centos6.4 x86_64 CD Install
* **Clobbers Disk**
* Works on my machines. 



Sources
=======
* https://github.com/okfn/ckan/wiki/How-to-Create-a-CentOS-Vagrant-Base-Box
* http://fedoraproject.org/wiki/Anaconda/Kickstart
* http://docs-v1.vagrantup.com/v1/docs/base_boxes.html
