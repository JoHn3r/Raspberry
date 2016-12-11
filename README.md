# Raspberry


-Send your pub key to the new server.
-Windows using Putty :
-type  public_id | plink.exe username@hostname "umask 077; test -d .ssh || mkdir .ssh ; cat >> .ssh/authorized_keys"
-Linux using OpenSSL:
-ssh-copy-id
-Disable the password
-/etc/ssh/sshd_config
