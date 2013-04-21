vagrant-centos64
================

A Vagrant kickstart file to provide the base necessities to create a personalized, vagrant basebox.

The VM's aren't guaranteed to be fully compliant, but this covers enough to enable me to build a base box, where I know the history of the base box. 

Purpose
-------

* A fast way to kickstart a CentOS base box. 
* Learning Vagrant


Gotchas
=======
* Assumes CD Install
* Clobbers Disk
* Works on my machines


Manual steps you need to do
---------------------------
* Install the VBoxLinuxAdditions
* Update UseDNS to no in /etc/ssh/sshd_config



Sources
=======
https://github.com/okfn/ckan/wiki/How-to-Create-a-CentOS-Vagrant-Base-Box
