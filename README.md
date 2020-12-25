# FuckingScanner
Fcuking scan bot list

# Firewalld
```
//add accept rules
firewall-cmd --get-zone-of-interface=eth0
firewall-cmd --zone=public --add-interface=eth0
firewall-cmd --zone=public --add-port=1-65535/tcp --permanent
firewall-cmd --zone=public --add-port=1-65535/udp --permanent
firewall-cmd --reload
// block fucking scanner bot
firewall-cmd --permanent --add-rich-rule="rule family='ipv4' source address='89.248.160.151/24' drop"
firewall-cmd --reload
```
