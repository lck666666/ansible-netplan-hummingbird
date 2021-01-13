# Ansible-network-config
Through ansible script, two network tools are provided to configure IPs for specified Linux machines.

## Supported Targets
The following Linux distros are tested:

Ubuntu 20.04

Centos 7

Other distros and versions may work too. If support for another distro is desired, submit an issue ticket. Pull requests are always welcome.

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

## Example in Lab
host1: ubuntu 20.04, 10.67.106.206

host2: centos 7,     10.67.107.97 

Use main.yml as playbook, for host1, because it uses netplan, the script can check it and config the network in netplan way. For host2, because it uses
NetworkManager, the script can check it and config the network in NetworkMangaer way.



