# dnsstatic_step
Make DNS IP address static

[root@node1 ~]# vim /etc/sysconfig/network-scripts/ifcfg-
ifcfg-enp0s3  ifcfg-lo
[root@node1 ~]# vim /etc/sysconfig/network-scripts/ifcfg-enp0s3
[root@node1 ~]# service network restart

TYPE=Ethernet
PROXY_METHOD=none
BROWSER_ONLY=no
BOOTPROTO=none
DEFROUTE=yes
IPV4_FAILURE_FATAL=no
IPV6INIT=no
IPV6_AUTOCONF=yes
IPV6_DEFROUTE=yes
IPV6_FAILURE_FATAL=no
IPV6_ADDR_GEN_MODE=stable-privacy
NAME=enp0s3
UUID=358262a9-73b0-4eee-a095-419126bb015f
DEVICE=enp0s3
ONBOOT=yes
IPADDR=192.168.1.32
PREFIX=24
GATEWAY=192.168.1.1
DNS1=192.168.1.1
