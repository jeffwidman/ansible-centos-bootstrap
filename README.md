CentOS Bootstrap role
=========

Ansible role that handles miscellaneous CentOS tasks like setting timezone,
grabbing yum updates, installing basic sysadmin tools, and enabling cron.

It's a catchall for anything that needs to happen when you first spin up a new
server that wasn't big enough to merit its own role.

Requirements
------------

Tested on CentOS 7 but should work on RHEL equivalents.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: centos-bootstrap, tags: ['bootstrap']}

License
-------

MIT

Author Information
------------------

Jeff Widman jeff@jeffwidman.com
