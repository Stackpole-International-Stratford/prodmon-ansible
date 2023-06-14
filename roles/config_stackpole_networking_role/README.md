Role Name
=========

A brief description of the role goes here.

Requirements
------------

None


Role Variables
--------------

Set in the host file: 
wanIP = (required) IP address to be assigned to eth0
lanIP = (required) IP address to be assigned to eth1
iplist = (optional) a list of internal ip adresses and the external ip addresses to map them to



Dependencies
------------

Example Playbook
----------------

Usage:
This role needs to be first in the playbook so it runs before anything else (required for apt):

- hosts: all
  tasks:

    - name: Include the example role and run its tasks
      include_role:
        name: config_stackpole_networking_role



License
-------

Author Information
------------------

Chris Strutton, cstrutton@stackpole.com