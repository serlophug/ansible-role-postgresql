Postgresql Role 
==================

Installs and configure Postgresql 9.6.

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows:
	
   ```postgresql_version ```: What version try to install. Default: ```9.6``` <br />
   ```postgresql_service_name```: Name of service. Default:```postgresql``` <br />
	```root_user```: Name and password of database user. Default: <br />
```yml
  root_user:
	   name: admin
      password: 1234	
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

