
<h2>Requirements</h2>
VirtualBox and Vagrant

<h2>Instructions</h2>

1. `git clone` or download the Vagrantfile to whatever directory you like and `cd` into it.

2. Download the CentOS 6.5 Vagrant box to that directory: 
https://www.dropbox.com/s/206lcenz3o45c79/centos65.box?dl=0 or 
http://benpiper.com/wp-content/uploads/2014/12/centos65.box.torrent

3. Add the CentOS 6.5 box: 
`vagrant box add centos65-base centos65.box`

4. Add the Ubuntu 14.04 64-bit box: 
vagrant box add https://vagrantcloud.com/ubuntu/boxes/trusty64

5. Launch the VMs: 
`vagrant up`