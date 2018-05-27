Ansible Role: compile-samba
===========================

This role does:

 - Install Samba from OS or from source (is this case, as recommended by [saba wiki](https://wiki.samba.org/index.php/Build_Samba_from_Source))
 - Setting systemd for smbd, nmbd, winbind and samba-ad-dc services

Role Variables
--------------

    install_samba_version: samba-4.8.2

Example Playbook
----------------

    - hosts: servers
      roles:
         - uspdev.install-samba
