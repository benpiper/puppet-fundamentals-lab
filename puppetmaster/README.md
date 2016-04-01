If you receive an error when installing Passenger, follow the instructions below immediately AFTER 3:33 into the "Installing Apache and Passenger" clip of the "Installing and Configuring the Puppet Master" module (https://app.pluralsight.com/player?course=puppet-system-administrators-fundamentals&author=ben-piper&name=puppet-system-administrators-fundamentals-m2&clip=10):

1. Install the Ruby Version Manager (RVM):

`\curl -sSL https://get.rvm.io | bash`

2. Restart root and vagrant shells:

`exit`

`exit`

`vagrant ssh`

3. Get back into a root shell:

`sudo su`

4. Install Ruby using RVM:

`rvm install ruby`

5. Install Passenger:

`gem install passenger`

`passenger-install-apache2-module`

Continue the course at 4:25 into the "Installing Apache and Passenger" clip.