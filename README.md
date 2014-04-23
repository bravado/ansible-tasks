Ansible Tasks
=============

Collection of tasks that can be included on ansible playbooks

Example yml
-----------

	---
	- hosts: all
	  user: vagrant

	  tasks:
	    - include: tasks/common.yml
	    - include: tasks/mongodb.yml
	    - include: tasks/oracle-java-7.yml
