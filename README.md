ansible-role-ius_yum_repo
=========================

Setup IUS yum repository for CentOS 7 as an Ansible-role.
https://ius.io/

Install role
------------

Create `requirements.yml` in your ansible playbook-folder.

    ---
    # Documentation:
    # https://docs.ansible.com/ansible/latest/reference_appendices/galaxy.html#installing-multiple-ro
....
....
    - name: tvartom.ius_yum_repo
      src: https://github.com/tvartom/ansible-role-ius_yum_repo
      scm: git
      # version: "v1.0" # Omit for latest version.

Run:

    $ ansible-galaxy install -r requirements.yml -p roles/


Requirements
------------

CentOS 7

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      tasks:
         - include_role:
             name: tvartom.ius_yum_repo

License
-------

CC-BY-4.0

Author Information
------------------

tvartom

