nomad
=========
Ansible role for [nomad](http://www.nomad.io/).
This role ensures that nomad runs as a daemon.

Requirements
------------
- unzip command on remote hosts

Role Variables
--------------
- datacenter (`local`)
- node\_name (`{{ ansible_hostname }}`)
- bootstrap_expect (0) - Equivalent to `-bootstrap-expect` command-line flag
- server (false) - Equivalent to `-server` command-line flag
- data\_dir (`/var/lib/nomad`) - Equivalent to `-data-dir` command-line flag

Dependencies
------------
No dependencies.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: tmtk75.nomad }

License
-------
MIT

Author Information
------------------
github: https://github.com/tmtk75  
twitter: https://twitter.com/tmtk75  
blog: http://blog.tmtk.net

