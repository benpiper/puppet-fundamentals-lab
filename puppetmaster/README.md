If you receive an error when installing Passenger, follow the instructions below immediately AFTER 3:33 into the "Installing Apache and Passenger" clip of the "Installing and Configuring the Puppet Master" module:

Install the Ruby Version Manager (RVM):
$ \curl -sSL https://get.rvm.io | bash

Restart root and vagrant shells:
$ exit
$ exit
$ vagrant ssh

Get back into a root shell:
$ sudo su

Install Ruby using RVM:
$ rvm install ruby

Install Passenger:
$ gem install passenger
$ passenger-install-apache2-module

Continue the course at 4:25 into the "Installing Apache and Passenger" clip.