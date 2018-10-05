Zabbix Dynamic Inventory
=======================

This script creates dynamic inventory with groups and hosts from zabbix.
All hosts have two variables:
- available (zabbix agent status)
- ansible_host (ip address)

Script creates two additional groups "group_all" and "Available_Zabbix_Agents".

Use group "Available_Zabbix_Agents" in LIMIT section to skip all unavailable hosts.

## Install
1. Copy zabbix.ini file to /etc/ansible/
2. Edit zabbix.ini with your parameters
3. Create custom script using zabbix.py

## Tested with
- Tower 3.2.5 (Ansible 2.6.4)
