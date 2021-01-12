# Ansible-network-config
Through ansible script, two network tools are provided to configure IPs for specified Linux machines.

## Ansible-netplan
In netplan_test, interface should be set up in vars file in advance. However, this way is not feasible in many cases. We'd better get the interface name from 
connected machines. 
In config_netplan.yml. We can get the interface name from connected machines, and then configure IP address to the specific one. IP address of each host should be set up in hosts file 
in advance.
## Ansible-nmcli
In nmcli_test, interface should be set up in vars file in advance. However, this way is not feasible in many cases. We'd better get the interface name from 
connected machines. 
In config_nmcli.yml. We can get the interface name and connection name of Network Manager from connected machines, and then configure IP address to the specific one. IP address of each host should be set up in hosts file 
in advance.


