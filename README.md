Consul
======

With this role it is possible to install [consul](https://consul.io) on a machine

Requirements
------------

None

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml) for the default values

    consul_required_packages
    
A list of packages which are required to install consul

    consul_user
    
User which should be used to run consul (will be created if not available)

    consul_group
    
Group which should be used for the consul_user (will be created if not available)

    consul_app_mirror

URL which should be used to download consul

    consul_app_platform
    
Platform on which consul should be installed (to be able to download the right package)

    consul_app_install_dir

Path which should be used to install consul

    consul_exec_path
    
Path which should be used for the executable

    consul_app
    
Name of the consul app itself (will be used to get the correct download url)

    consul_app_version
    
Version which should be installed

    consul_app_checksum
    
Checksum of the version

    consul_app_name
    
App name which will be used to build the correct download url

    consul_app_zip
    
Zip filename which will be used to build the correct download url

    consul_app_url
    
Template to build the correct download url

    consul_configuration_path
    
Path which should be used to store configurations for consul

    consul_app_download_location
    
Temporary download location which will be used to download the application

Dependencies
------------

None

Example Playbook
----------------

    - hosts: consuls
          roles:
             - solutionDrive.consul

License
-------

MIT

Author Information
------------------

solutionDrive GmbH (info@solutiondrive.de)
