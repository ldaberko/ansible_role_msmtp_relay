msmtp-relay
=========

Installing and setting up msmtp to relay mail using third party smtp servers.

Requirements
------------

The FreeBSD sysrc requires community.general version 2.5.9

Role Variables
--------------

user - login for smtp relay account, usually your email address

password - password for the above account

msmtp_login.yml is stored outside the role directory structure
usually in ansible/vars and is usually an ansible vault with 
user and password login information

Example Playbook
----------------

    - hosts: servers
      roles:
         - msmtp-relay

License
-------

GPLv3

