[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Build Status](https://travis-ci.org/serlophug/ansible-role-postgresql.svg?branch=master)](https://travis-ci.org/serlophug/ansible-role-postgresql)

Postgresql Role 
==================

Installs and configure Postgresql 9.6.

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows:
	
   ```postgresql_version```: Version to install (see which supports in /meta/main.wml).<br /> 
   ```postgresql_service_name```: Service name. <br />
	```db_name```: Database name. <br />
	```create_db```: Whether or not create database "db_name". <br />
   ```root_user```: Name and password of database user. <br /><br />
   Default values:
```yml
  postgresql_version: 9.6
  postgresql_service_name: postgresql
  db_name: database
  create_db: yes
  root_user:
      name: postgres
      password: default,	
```

Example Playbook
----------------


```yml
  roles:
    - { role: 'serlophug.postgresql'}
```


License
-------

Apache Licence v2 [1]

[1] http://www.apache.org/licenses/LICENSE-2.0

