Resolvfile Role
=========

This roles purpose is to configure the `/etc/resolv.conf` file.

[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-neoloc.resolvfile-blue.svg)](https://galaxy.ansible.com/neoloc/ansible-role-resolvfile/)

Requirements
------------

All included in ansible-base package.

Role Variables
--------------

| Variable                | Required | Default | Choices                   | Comments                                 |
|-------------------------|----------|---------|---------------------------|------------------------------------------|
| resolvfile.searchdomain   | no       | N/A     | string value              | searchdomain to be set in /etc/resolv.conf |
| resolvfile.forwarders     | no       | 8.8.8.8 | list of IP addresses      | nameservers to be set in /etc/resolv.conf  |

```yaml
resolvfile:
  searchdomain: somedomain.tld
  forwarders:
    - 1.1.1.1
    - 9.9.9.9
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - neoloc.resolvfile

License
-------

See license.md

Author Information
------------------

[![Github](https://img.shields.io/badge/Github-neoloc-blue.svg)](https://github.com/neoloc)
