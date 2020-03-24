Role Name
=========

A simple Role which ensure that a list of services are in a given state

Requirements
------------

None

Role Variables
--------------

svc_status_services_list: List of services we want to manage

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
	 - role: erwstx.svc_status
	   svc_status_services_list:
	   - name: puppet
	     state: started
	   - name: firewalld
	     state: stopped

License
-------

BSD

Author Information
------------------

erwstx@GitHub
