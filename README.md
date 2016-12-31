<h1>Vagrantfiles for the Puppet Fundamentals for System Administrators course</h1>

<h2>Vagrant Box Downloads for VirtualBox</h2>
<b>CentOS 6.5</b>:

Torrent (recommended): http://benpiper.github.io/course-files/puppet-system-administrators-fundamentals/centos65.box.torrent
<br>
<i>NB: If you download the torrent, please seed it for at least a couple of days so others can download the image faster.</i>

Dropbox: https://www.dropbox.com/s/206lcenz3o45c79/centos65.box?dl=1

<b>Ubuntu 14.04 LTS</b>: http://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box

<h2>Requirements</h2>
VirtualBox and Vagrant

Note for RHEL/CentOS Linux users: You may need to run the following commands after installing VirtualBox:

`sudo yum -y install kernel-devel`<br>
`sudo /etc/init.d/vboxdrv setup`

<h2>Lab Setup Instructions</h2>

1. `git clone` this repository or download `master.zip` and unzip to the `puppet-fundamentals-lab` directory and `cd` to it.

2. Download the CentOS 6.5 Vagrant box to the `puppet-fundamentals-lab` directory: 
https://www.dropbox.com/s/206lcenz3o45c79/centos65.box?dl=1 or<br> 
http://benpiper.github.io/course-files/puppet-system-administrators-fundamentals/centos65.box.torrent<br>
Ensure the file is saved as `centos65.box`.

3. Add the CentOS 6.5 box you just downloaded:
`vagrant box add centos65-base centos65.box`

4. Download the Ubuntu 14.04 Vagrant box to the same directory:
http://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box

5. Add the Ubuntu box:
`vagrant box add trusty64 trusty-server-cloudimg-amd64-vagrant-disk1.box`

<h2>Booting the Puppet Master Server</h2>

1. `cd` into the `puppetmaster` subdirectory and launch the VM:
`vagrant up`

2. Once the machine is booted, SSH into it:
`vagrant ssh`

<h2>Windows 2008 R2 ISO</h2>
http://www.microsoft.com/en-us/download/details.aspx?id=11093
