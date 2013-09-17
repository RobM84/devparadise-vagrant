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
  * apache2 => git@github.com:opscode-cookbooks/apache2.git
  * apt => git@github.com:opscode-cookbooks/apt.git
  * aws => git@github.com:opscode-cookbooks/aws.git
  * build-essential => git@github.com:opscode-cookbooks/build-essential.git
  * chef_handler => git@github.com:opscode-cookbooks/chef_handler.git
  * database => git@github.com:opscode-cookbooks/database.git
  * dmg => git@github.com:opscode-cookbooks/dmg.git
  * git => https://github.com/opscode-cookbooks/git
  * mysql => git@github.com:opscode-cookbooks/mysql.git
  * openssl => git@github.com:opscode-cookbooks/openssl.git
  * php => git@github.com:opscode-cookbooks/php.git
  * postgresql => git@github.com:opscode-cookbooks/postgresql.git
  * runit => git@github.com:opscode-cookbooks/runit.git
  * vagrant_magento => git@github.com:RobM84/vagrant_magento.git
  * windows => git@github.com:opscode-cookbooks/windows.git
  * xfs => git@github.com:opscode-cookbooks/xfs.git
  * xml => git@github.com:opscode-cookbooks/xml.git
  * yum => git@github.com:opscode-cookbooks/yum.git
1. Do a `vagrant up` from the base folder
