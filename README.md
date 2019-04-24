# Raspberry


 - Send your pub key to the new server.
 - Windows using Putty :
 - type  public_id | plink.exe username@hostname "umask 077; test -d .ssh || mkdir .ssh ; cat >> .ssh/authorized_keys"
 - Linux using OpenSSL:
 - ssh-copy-id
 - Disable the password
 - /etc/ssh/sshd_config
 
 @reboot script
 amixer sset Speaker,0 100%,100% unmute

>check network :

```sh
$ for i in $(seq 1 255) ;do ping -q -w 1 -c 1 192.168.1.$i | grep "100% packet loss" > /dev/null || echo "192.168.1.$i is alive"; done
```

[Online Markdown Editor](https://dillinger.io/)
