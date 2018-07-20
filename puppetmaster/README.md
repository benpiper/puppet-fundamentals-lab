If you receive an error when installing Passenger, follow the instructions below immediately AFTER 3:33 into the "Installing Apache and Passenger" clip of the "Installing and Configuring the Puppet Master" module:

0. (Optional) From your host machine, take a snapshot: `vagrant snapshot save puppetmaster`
1. Install the following: `sudo gem install rake --version 10.4.2`
                           `sudo gem install rack --version 1.6.0`
                          `sudo gem install passenger --version 4.0.56`
                          `sudo gem install daemon_controller --version 1.2.0`
2. Install the Passenger Apache module: `sudo passenger-install-apache2-module`

Continue the course at 4:25 into the "Installing Apache and Passenger" clip (https://app.pluralsight.com/player?course=puppet-system-administrators-fundamentals&author=ben-piper&name=puppet-system-administrators-fundamentals-m2&clip=10)

If you receive an error when running the puppet agent on the wiki server after installing puppetlabs-apache during the Module "Creating and Using Modules", section "The Apache Module", follow the instructions below

1. Uninstall the version of puppetlabs-apache that was installed: 
  `sudo puppet module uninstall puppetlabs-apache --modulepath /etc/puppet/environments/production/modules/`
2. Install puppetlabs-apache version 1.2: 
  `sudo puppet module uninstall puppetlabs-apache --modulepath /etc/puppet/environments/production/modules/ --version 1.2.0`
3. Uninstall puppetlabs-concat and install puppetlabs-concat 1.1.2: 
  `sudo puppet module uninstall puppetlabs-concat --modulepath /etc/puppet/environments/production/modules/ --force`  
  `sudo puppet module install puppetlabs-concat --modulepath /etc/puppet/environments/production/modules/ --version 1.1.2`
4. Uninstall puppetlabs-stdlib and install puppetlabs-stdlib 4.5.0
  `sudo puppet module uninstall puppetlabs-stdlib --modulepath /etc/puppet/environments/production/modules/ --force`
  `sudo puppet module install puppetlabs-stdlib --modulepath /etc/puppet/environments/production/modules/ --version 4.5.0`
  
Continue the course at 10:41 into the "The Apache Module" clip.
