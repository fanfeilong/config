+ chkconfig
  - chkconfig iptables on
  - chkconfig iptables off
+ restart 
  - service iptables stop
  - service iptables start
  - service iptables restart
+ modify
  - `vim /etc/sysconfig/iptables`
  - `-A RH-Firewall-1-INPUT -m state --state NEW -m multiport -p tcp --dport from:to -j ACCEPT` 
  - `-A RH-Firewall-1-INPUT -m state --state NEW -m multiport -p udp --dport from:to -j ACCEPT`