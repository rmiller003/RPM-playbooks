Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

    netscaler_url: https://netscaler.citrix.com
    nitro_username: nitro_user
    nitro_password: nitro_pass

| Variable Name | Required | Default | Description | Example |
| --- | --- | --- | --- | --- |
| netscaler_url | yes | None | URL or IP of Citrix Netscaler device | https://netscaler.citrix.com | 
| nitro_username | yes | None | Nitro API User | nitro_user |
| nitro_password | yes | None | Nitro API Password | nitro_pass |
| backend_servers | yes | None | List of backend servers | | 
| service_group_name | yes |  None | Name of service group where backend servers are to be added | service-group-1 | 
| service_group_type | no | HTTP |  | HTTP | 
| lb_monitor_name | yes | None | Name of load balancing monitor | monitor_1 | 
| lb_monitor_type | no | HTTP-EVC | |
| lb_vserver_name | yes | None | |
| lb_service_type | no | HTTP | |
| loadbalancing_method | no | ROUNDROBIN | | | 

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
