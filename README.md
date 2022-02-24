set_proxy4rhsm
==============

With this role you can configure subscription-manager to use a
reverse proxy to access the subscription management. The proxy
configuration is set in /etc/rhsm.conf.

Requirements
------------

None.

Role Variables
--------------

Variables with default values are defined in `defaults/main.yml`:

```yaml
set_proxy4rhsm_proxy_hostname: "proxy.example.com" # Sets proxy address using FQDN or IP
set_proxy4rhsm_proxy_port: "3128"
```

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - role: set_proxy4rhsm
          vars:
            set_proxy4rhsm_proxy_hostname: "proxy.example.com"
            set_proxy4rhsm_proxy_port: "3128" 

License
-------

MIT

Author Information
------------------

Author: Joerg Kastning (Tronde)
