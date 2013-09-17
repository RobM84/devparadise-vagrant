Vagrant with Magento
====================

## Description
On `vagrant up`, a Magento test environment is provisioned using apache2, mysql5, php and whatever Magento version you put into the `magento`folder. The sample data is downloaded and added on the first run. As soon as a `local.xml` file exists in the `./magento/app/etc/` folder, the Magento installation and import of sample data are skipped.  

The [master branch](https://github.com/RobM84/devparadise-vagrant/tree/master) only keeps the Vagrant file and the basic structure, all Chef cookbooks need to be downloaded separately. There is a [quickstart branch](https://github.com/RobM84/devparadise-vagrant/tree/quickstart) containing all Chef cookbooks, please not these cookbooks won't be updated to newer versions. 

### Magento configuration
http://127.0.0.1:1080/    
http://127.0.0.1:1080/admin/    
Admin User: mage-admin    
Admin Password: abc1234    
 

## Structure
./deploy_support/chef/cookbooks/    
./deploy_support/chef/roles/magento_dev.rb    
./magento/    
./Vagrantfile    
 
## How To
### Quickstart
1. Download & install VirtualBox => https://www.virtualbox.org/wiki/Downloads
1. Download & install Vagrant => http://downloads.vagrantup.com/
1. Download Magento => http://www.magentocommerce.com/download
1. Extract Magento into `./magento/` directory
1. Do a `vagrant up` from the base folder

### Full version
1. Download & install VirtualBox => https://www.virtualbox.org/wiki/Downloads
1. Download & install Vagrant => http://downloads.vagrantup.com/
1. Download Magento => http://www.magentocommerce.com/download
1. Extract Magento into `./magento/` directory
1. Checkout the following Chef cookbooks into `./deploy_support/chef/cookbooks/` directory
  * apache2 => [git@github.com:opscode-cookbooks/apache2.git](git@github.com:opscode-cookbooks/apache2.git)
  * apt => [git@github.com:opscode-cookbooks/apt.git](git@github.com:opscode-cookbooks/apt.git)
  * aws => [git@github.com:opscode-cookbooks/aws.git](git@github.com:opscode-cookbooks/aws.git)
  * build-essential => [git@github.com:opscode-cookbooks/build-essential.git](git@github.com:opscode-cookbooks/build-essential.git)
  * chef_handler => [git@github.com:opscode-cookbooks/chef_handler.git](git@github.com:opscode-cookbooks/chef_handler.git)
  * database => [git@github.com:opscode-cookbooks/database.git](git@github.com:opscode-cookbooks/database.git)
  * dmg => [git@github.com:opscode-cookbooks/dmg.git](git@github.com:opscode-cookbooks/dmg.git)
  * git => [https://github.com/opscode-cookbooks/git](https://github.com/opscode-cookbooks/git)
  * mysql => [git@github.com:opscode-cookbooks/mysql.git](git@github.com:opscode-cookbooks/mysql.git)
  * openssl => [git@github.com:opscode-cookbooks/openssl.git](git@github.com:opscode-cookbooks/openssl.git)
  * php => [git@github.com:opscode-cookbooks/php.git](git@github.com:opscode-cookbooks/php.git)
  * postgresql => [git@github.com:opscode-cookbooks/postgresql.git](git@github.com:opscode-cookbooks/postgresql.git)
  * runit => [git@github.com:opscode-cookbooks/runit.git](git@github.com:opscode-cookbooks/runit.git)
  * vagrant_magento => [git@github.com:RobM84/vagrant_magento.git](git@github.com:RobM84/vagrant_magento.git)
  * windows => [git@github.com:opscode-cookbooks/windows.git](git@github.com:opscode-cookbooks/windows.git)
  * xfs => [git@github.com:opscode-cookbooks/xfs.git](git@github.com:opscode-cookbooks/xfs.git)
  * xml => [git@github.com:opscode-cookbooks/xml.git](git@github.com:opscode-cookbooks/xml.git)
  * yum => [git@github.com:opscode-cookbooks/yum.git](git@github.com:opscode-cookbooks/yum.git)
1. Do a `vagrant up` from the base folder

