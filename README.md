Vagrant PHP box
===============

This box was made for personal use (puppet scripts generated using puphpet.com).

## Requirements
* [Vagrant 1.4+](http://www.vagrantup.com/downloads.html)
* [VirtualBox 4.3+](https://www.virtualbox.org/wiki/Downloads)

## Vagrant shared folders
* Box folder /var/www/vhosts is mapped to ~/Development, good luck if you're on windows.

## Box config (Debian Wheezy 7.2 x64)
* Network IP: 192.168.2.254
* VM RAM 512M
* Apache2 with 3 vhosts pre-setup: laravel.dev, wordpress.dev, drupal.dev
* PHP 5.5 (upload and memory limit set to 512M)
* XDebug (debug port mapped to 10000)
* Drush 6.x
* MySQL 5.5.x with 3 databases: laravel, wordpress, drupal (root pw: mysqlroot)
* MongoDB running on 27017 (mapped to port 11000)
* Redis running on 6379 (mapped to port 12000)
* Beanstalkd running on 13000 (mapped to port 13000)

## Box utilities
* phpMyAdmin on http://192.168.2.254/phpmyadmin
* Beanstalkd console on http://192.168.2.254/beanstalk_console/public/

# Scripts (todo)
Add command line bash script to create/add a vhost in the vagrant machine.
This script should also be able to install laravel, drupal and wordpress distributions automatically.
