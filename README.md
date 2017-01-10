cliff
=========

This role provides the [CLIFF geoparser](http://cliff.mediameter.org)
as a systemd service, accessible on localhost via HTTP.

Requirements
------------

This role was developed on Ubuntu 16.04 and assumes a
few packages are available via apt, 
see the list of packages in `vars/main.yml`.

Role Variables
--------------

- `cliff_home`: root containing Tomcat, Clavin & Cliff (default `/opt/cliff`)
- `tomcat_port`: port on which Tomcat serves e.g. Cliff (default `8005`)

Dependencies
------------

No dependencies on other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: maedoc.cliff, cliff_home: /usr/local/cliff, tomcat_port: 8042 }

License
-------


Author Information
------------------

