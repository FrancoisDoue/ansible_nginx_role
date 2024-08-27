Role Name
=========

Exercise role to install nginx

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------
Exposed ports for nginx server
```yml
nginx_port: 80
``` 
Default configuration files
```yml
default_files:
  - "/etc/nginx/sites-available/default"
  - "/etc/nginx/sites-enabled/default"
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yml
hosts: servers
roles:
  - nginx
```

