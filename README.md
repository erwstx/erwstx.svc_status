Role Name
=========

A simple Role which ensure that a list of services are in a given state

Requirements
------------

N/A

Role Variables
--------------

svc_status_services_list: List of services we want to manage

Dependencies
------------

N/A

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
