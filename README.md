Lean repository for Vagrant with Magento
========================================

## Description
The repository only keeps the Vagrant file and the basic structure, all Chef cookbooks need to be downloaded separately.

## Structure
./deploy_support/chef/cookbooks/    
./deploy_support/chef/roles/magento_dev.rb    
./magento/    
./Vagrantfile    
 
## How To
1. Download & install VirtualBox => https://www.virtualbox.org/wiki/Downloads
1. Install Vagrant => http://downloads.vagrantup.com/
1. Download Magento => http://www.magentocommerce.com/download
1. Extract Magento into `./magento/` directory
1. Checkout the following Chef cookbooks into `./deploy_support/chef/cookbooks/` directory
  * apache2
  * apt
  * aws
  * build-essential
  * chef_handler
  * database
  * dmg
  * git
  * mysql
  * openssl
  * php
  * postgresql
  * runit
  * vagrant_magento
  * windows
  * xfs
  * xml
  * yum 

