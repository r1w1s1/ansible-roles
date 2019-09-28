SFTP-Server
=========

Setup SFTP-Server on CentOS 7 with chroot support


Role Variables
--------------

* `sftp_group`: sftpusers
* `sftp_users`: test
* `pass`: $1$ChwuF/kz$T9VFRaO.rgFU./KcPecSe/

Can use the python to generate the password.

`python -c 'import crypt; print crypt.crypt("password", "$1$SomeSalt$")'`


Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ricardson.sftp-chroot }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
