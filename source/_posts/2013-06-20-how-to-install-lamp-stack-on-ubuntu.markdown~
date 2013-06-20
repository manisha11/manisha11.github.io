---
layout: post
title: "How to Install LAMP Stack on Ubuntu"
date: 2013-06-20 13:23
comments: true
categories: 
author: Manisha
---
LAMP stack is a group of open source software used to get web servers up and running. 
The acronym stands for Linux, Apache, MySQL, and PHP.

Set Up:-


Step One—Install Apache
Apache is a free open source software which runs over 50% of the world’s web servers.

To install apache, open terminal and type in these commands:
sudo apt-get update
sudo apt-get install apache2

That’s it. To check if Apache is installed, direct your browser to your server’s IP (eg. http://12.34.56.786).The page should display the words "Success"

How to Find your Server’s IP address:-
To reveal your server's IP address type in the following command.
ifconfig eth0|grep inet|awk '{print $2}'



Step Two—Install MySQL

MySQL is a powerful database management system used for organizing and retrieving data 

To install MySQL, open terminal and type in these commands:

sudo apt-get install mysql-server libapache2-mod-auth-mysql php5-mysql

Once you have installed MySQL, we should activate it with this command: 

sudo mysql_install_db

Finish up by running the MySQL set up script:

sudo /usr/bin/mysql_secure_installation

The prompt will ask for the current root password.


Type it in.

Enter current password for root (enter for none): 
OK, successfully used password, moving on...


Then the prompt will ask you if you want to change the root password. Go ahead and choose N and move on to the next steps.

It’s easiest just to say Yes to all the options. At the end, MySQL will reload and implement the new changes.

By default, a MySQL installation has an anonymous user, allowing anyone
to log into MySQL without having to have a user account created for
them.  This is intended only for testing, and to make the installation
go a bit smoother.  You should remove them before moving into a
production environment.

Remove anonymous users? [Y/n] y                                            
 ... Success!

Normally, root should only be allowed to connect from 'localhost'.  This
ensures that someone cannot guess at the root password from the network.

Disallow root login remotely? [Y/n] y
... Success!

By default, MySQL comes with a database named 'test' that anyone can
access.  This is also intended only for testing, and should be removed
before moving into a production environment.

Remove test database and access to it? [Y/n] y
 - Dropping test database...
 ... Success!
 - Removing privileges on test database...
 ... Success!

Reloading the privilege tables will ensure that all changes made so far
will take effect immediately.

Reload privilege tables now? [Y/n] y
 ... Success!




Step Three—Install PHP:
PHP is an open source web scripting language that is widely use to build dynamic webpages.
 
To install PHP, open terminal and type in this command.

sudo apt-get install php5 libapache2-mod-php5 php5-mcrypt

It may also be useful to add php to the directory index, to serve the relevant php index files:

sudo nano /etc/apache2/mods-enabled/dir.conf

Add index.php to the beginning of index files.Now the page should now look like this:

<IfModule mod_dir.c>

          DirectoryIndex index.php index.html index.cgi index.pl index.php index.xhtml index.htm

</IfModule>

PHP Modules

PHP also has a variety of useful libraries and modules that you can add onto your virtual server. You can see the libraries that are available. 
apt-cache search php5-


Terminal will then display the list of possible modules. The beginning looks like this:

php5-cgi - server-side, HTML-embedded scripting language (CGI binary)
php5-cli - command-line interpreter for the php5 scripting language
php5-common - Common files for packages built from the php5 source
php5-curl - CURL module for php5
php5-dbg - Debug symbols for PHP5
php5-dev - Files for PHP5 module development
php5-gd - GD module for php5
php5-gmp - GMP module for php5
php5-ldap - LDAP module for php5
php5-mysql - MySQL module for php5
php5-odbc - ODBC module for php5
php5-pgsql - PostgreSQL module for php5
php5-pspell - pspell module for php5
php5-recode - recode module for php5
php5-snmp - SNMP module for php5
php5-sqlite - SQLite module for php5
php5-tidy - tidy module for php5
php5-xmlrpc - XML-RPC module for php5
php5-xsl - XSL module for php5
php5-adodb - Extension optimising the ADOdb database abstraction library
php5-auth-pam - A PHP5 extension for PAM authentication
[...]

Once you decide to install the module, type:

sudo apt-get install name of the module


You can install multiple libraries at once by separating the name of each module with a space.

NOW THE LAMP STACK IS SUCCESSFULLY INSTALLED.



