## zabbix-spk

Zabbix Synology spk for differents models. Please have a look on different branchs for latest Zabbix version

# -----------------------------
For DSM 7.0 MUST BE INSTALLED TWICE TO CREATE APPROPRIATE INSTALLAION SINCE SECURITY PB 
# -----------------------------

On DSM7.0, must apply manually as root after installation to have icmping items working
		
		#> chown root:synocommunity /var/packages/zabbix/target/sbin/fping<br>
		#> chmod 4710 /var/packages/zabbix/target/sbin/fping

Since Zabbix 6.2.8, ZBX-22588, only HTTP, HTTPS protocols are supported in web scenarios. This package includes FTP and RSTP protocols support


It consists of Zabbix server, Zabbix Proxy and Zabbix agent and uses the Synology supplied mysql/mariadb datbase server. 
Package is build to run only one Zabbix Server OR one Zabbix Proxy, but not Zabbix Server and proxy on the same time.

Please ask in case your package is not available.

This branch is 6.4.1. Under construction. 
I'm currently working on 6.4.1 packages.
But from now, I have some troubles with web scenarios in this new version.

I had the answer from zabbix. Problem was appearing since 6.2.8. ZBXNEXT-9015 was created.
I discovered where to add other protocols in 6.4.x. So I could restart to provide new updates.


Big Hugs
Camille


https://www.zabbix.com/whats_new_6_4
https://www.zabbix.com/documentation/6.4



Live from Zabbix 
https://www.youtube.com/user/ZabbixSIA

Link on Zabbix wiki about synology
https://zabbix.org/wiki/InstallOnSynology#Install_the_spk
