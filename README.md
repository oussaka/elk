ELK setup
=========

Role setup and configure elasticsearch, nginx, kibana, logstash


Role Variables
--------------

	kibana_server_name: "" - server name for kibana
	htpasswords: "" - login and password for basic auth 

Example Playbook
----------------

	---
	- hosts: sphetz
	  become: yes
	  roles: 
	    - { role: "dolbager.elk", kibana_server_name: "logs.you.domain.com", htpasswords: {name: "login", pass: "password"}}

