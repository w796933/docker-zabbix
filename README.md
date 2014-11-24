Docker Zabbix
========================

I found that I needed to modify the berngp/docker-zabbix image
to change some settings for the zabbix server and do some
MySQL database optimizations.  Without these changes, the
Zabbix server process kept dying and the monit process kept
starting it.  The main issue was the Zabbix cache usage dropping
below 20% free.

![alt tag](https://raw.githubusercontent.com/CosmicQ/docker-zabbix/master/before-after.png)
