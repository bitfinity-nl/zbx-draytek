# zbx-draytek
Zabbix template for monitoring Draytek router/Firewall

Requirements
------------

* Zabbix 4.0 or higher
* Draytek router/firewall

Howto
------------

* Import the zbx-draytek template to the Zabbix server before proceeding.

On Zabbix
1. Create new host in Zabbix and add the "ip address" or "dns name" to the SNMP interfaces.
2. Navigate to templates and add the template "zbx-draytek" as a linked template to the host.
3. Navigate to "Macros" and add set the macro {$SNMP_COMMUNITY} with value the desired community string (default: public).

On Draytek
1. Enable SNMP and set the desired community string.
