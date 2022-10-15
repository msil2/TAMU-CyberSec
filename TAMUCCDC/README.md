# Public Tutorials

[https://github.com/Forty-Bot/linux-checklist/blob/master/README.md](https://github.com/Forty-Bot/linux-checklist/blob/master/README.md)

[https://ostechnix.com/find-files-based-permissions/](https://ostechnix.com/find-files-based-permissions/)

[https://manpages.ubuntu.com/manpages/trusty/man8/ufw.8.html](https://manpages.ubuntu.com/manpages/trusty/man8/ufw.8.html)

[https://www.tecmint.com/block-ping-icmp-requests-to-linux/](https://www.tecmint.com/block-ping-icmp-requests-to-linux/)

[https://www.linuxtechi.com/enforce-password-policies-linux-ubuntu-centos/](https://www.linuxtechi.com/enforce-password-policies-linux-ubuntu-centos/)

[https://qr.ae/pvJPV5](https://qr.ae/pvJPV5)

[https://ostechnix.com/how-to-set-password-policies-in-linux/](https://ostechnix.com/how-to-set-password-policies-in-linux/)

[https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-security-configuration-framework/security-compliance-toolkit-10](https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-security-configuration-framework/security-compliance-toolkit-10)

[https://www.youtube.com/watch?v=hum4hzNE_j8&list=PLRNX6rCpHwNys6o-_z2R1FTlr_cn5FRKw&index=4](https://www.youtube.com/watch?v=hum4hzNE_j8&list=PLRNX6rCpHwNys6o-_z2R1FTlr_cn5FRKw&index=4)

[https://www.computerworld.com/article/3144985/linux-hardening-a-15-step-checklist-for-a-secure-linux-server.html](https://www.computerworld.com/article/3144985/linux-hardening-a-15-step-checklist-for-a-secure-linux-server.html)

[https://qr.ae/pvJkf5](https://qr.ae/pvJkf5)

[https://phoenixnap.com/kb/how-to-list-display-view-all-cron-jobs-linux](https://phoenixnap.com/kb/how-to-list-display-view-all-cron-jobs-linux)

[https://docs.oracle.com/cd/E23824_01/html/821-1451/sysrescron-24589.html](https://docs.oracle.com/cd/E23824_01/html/821-1451/sysrescron-24589.html)

[https://github.com/ucrcyber/hivestorm/blob/main/linux_users.sh](https://github.com/ucrcyber/hivestorm/blob/main/linux_users.sh)

```
netstat -nutlp
lsof -i
systemctl
id ACCOUNT
userdel -r
find / -user UID
find / -nouser
nc -v HOST PORT
/etc/ssh/sshd_config
DenyUsers account1 accountN
PermitRootLogin no
Banner none
PasswordAuthentication no
PubkeyAuthentication yes
PermitRootLogin no 
AllowTcpForwarding no
GatewayPorts no
Port 2222
systemctl reloadsshd
awk -F: '($3 == "0") {print}' /etc/passwd
~/.ssh/authorized_keys
pam_securetty: auth [user_unknown=ignore success=ok ignore=ignore default=bad] securetty.so
/etc/securetty
```

