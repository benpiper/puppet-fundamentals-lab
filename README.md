<h1>Vagrantfile for the Puppet Fundamentals for System Administrators course</h1>

<h2>Requirements</h2>
VirtualBox and Vagrant

<h2>Instructions</h2>

1. `git clone` or download the directories to whatever parent directory you like and `cd` into the parent.

2. Download the CentOS 6.5 Vagrant box to the parent directory: 
https://www.dropbox.com/s/206lcenz3o45c79/centos65.box?dl=1 or 
http://benpiper.com/wp-content/uploads/2014/12/centos65.box.torrent

3. Add the CentOS 6.5 box you just downloaded:
`vagrant box add centos65-base centos65.box`

4. Add the Ubuntu 14.04 64-bit box from the Vagrant cloud:
`vagrant box add https://vagrantcloud.com/ubuntu/boxes/trusty64`

5. `cd` into each directory and launch the VMs: 
`vagrant up`
