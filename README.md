Postgresql Role 
==================

Installs and configure Postgresql 9.6.

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows:
	
   ```postgresql_version```: Version to install (see which supports in /meta/main.wml).<br /> 
   ```postgresql_service_name```: Service name. <br />
   ```root_user```: Name and password of database user. <br /><br />
   Default values:
```yml
  postgresql_version: 9.6
  postgresql_service_name: postgresql
  root_user:
      name: postgres
      password: postgres-.,	
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

