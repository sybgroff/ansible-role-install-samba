Ansible Role: compile-samba
===========================

This role executes tasks:

 - Build Samba from Source as recommended by [saba wiki](https://wiki.samba.org/index.php/Build_Samba_from_Source), for now, to Ubuntu Xenial
 - Create a service to start, stop and restart samba
 - Insert executable bins from samba compiled on /usr/local/sbin 

Role Variables
--------------

    samba_version: samba-4.4.8
    samba_path: /usr/local/samba
    download: /opt

Example Playbook
----------------

    - hosts: servers
      roles:
         - uspdev.compile-samba
