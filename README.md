Role Name
=========

This Ansible role provisions a docker on a Mac OSX computer & configuring it's networking WITHOUT the need supply the administrator password via the GUI.

Requirements
------------

The role must be run as a superuser. e.g.

~~~~
ansible-playbook -i "localhost," -c local tests/test.yml --ask-sudo-pass
~~~~

Dependencies
------------

This role uses homebrew to install apps, therefore has a dependency upon the geerlingguy.homebrew role.

Example Playbook
----------------

	---
	- hosts: localhost
	  remote_user: root
	  roles:
	    - sicruse.macdocker

License
-------

MIT

Author Information
------------------

If you have any questions or comments feel free to reach me via [email](mailto:si@sicruse.com?subject=macdocker%20Feedback)
