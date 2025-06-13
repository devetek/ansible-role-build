Ansible role: Build
=========

This Ansible role automates the process of building a specified application from source or predefined configuration. It handles environment setup, dependency installation, compilation/build tasks, and optional artifact packaging. It also supports reading application-specific configuration from a YAML-based DSL file, allowing declarative and centralized configuration management.

Requirements
------------

None.

Role Variables
--------------

List of variables in ansible-role-build:

```sh
---
build_id: 0
build_appname: ""
build_upload_artifact: false
build_user: root
build_destination: "/opt"
build_log: "/va/log/"

build_application:

build_application_from_input: ""
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - devetek.build
```

License
-------

GNU General Public License v3.0 or later

Author Information
------------------

[Nedya Prakasa]. Role created for [dPanel].

[dPanel]: https://cloud.terpusat.com/
[Nedya Prakasa]: https://github.com/prakasa1904
[devetek]: https://github.com/devetek
[geerlingguy.php]: https://galaxy.ansible.com/ui/standalone/roles/geerlingguy/php/
[geerlingguy.composer]: https://galaxy.ansible.com/ui/standalone/roles/geerlingguy/composer/