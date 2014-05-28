Ansible Tasks
=============

Collection of tasks that can be included on ansible playbooks


Example Vagrantfile
-------------------

    config.vm.provision "ansible" do |ansible|
        ansible.raw_arguments = "-i hosts"
        ansible.playbook = "server.yml"
    end

Example yml
-----------

	---
	- hosts: all
	  user: vagrant

	  tasks:
	    - include: tasks/common.yml
	    - include: tasks/mongodb.yml
	    - include: tasks/oracle-java-7.yml
