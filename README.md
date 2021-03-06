# Titan graph DB Chef Cookbook

Installs Titan embedded within cassandra + connects to elastic search as index backend

## Tested OS Distributions

Ubuntu 12.04.


## Recipes

Default: Install Titan embedded with cassandra and connect to existing elastic search index backend. See attributes for configuration options. 


## Dependencies

Cookbook dependecies managed by Berkshelf (see Berskfile)

##Vagrant test cluster usage

1. Install [Vagrant](http://www.vagrantup.com/)
2. Install [Berkshelf](http://berkshelf.com/)
3. Add vm image to vagrant: cookbook_root$  vagrant box add precise64 http://files.vagrantup.com/precise64.box
4. cookbook_root$ vagrant plugin install vagrant-omnibus
5. cookbook_root$ vagrant plugin install vagrant-berkshelf
6. cookbook_root$ berks install
7. cookbook_root$ vagrant up

Vagrant should launch a titan node and an elastic search node for you to test out.


##TODO
1. Fleshout documentation
2. Add support for more titan options
3. Add support for HBASE

## Copyright & License

Brian Cajes, 2013

Released under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0.html).
