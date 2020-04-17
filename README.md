Ansible Role: NFS Client
========================

[![Build Status](https://travis-ci.org/diadzine/ansible-role-nfs-client.svg?branch=master)](https://travis-ci.org/diadzine/ansible-role-nfs-client)

Ansible role for NFS client installation.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

NFS shares:

    nfs_shares: []

Example of configuration:

    nfs_shares:
      - share: "server:/nfs/share"
        mount_point: /mnt/share
        mount_opts: hard,nolock
        mount_owner: root
        mount_group: sudo

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: server
      roles:
         - { role: ansible-role-nfs-client }

License
-------

MIT License.

Author Information
------------------

This role was created in 2020 by [Aymeric Bringard](https://github.com/diadzine/).
