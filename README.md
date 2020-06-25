# Hub-Spoke

•	JSON includes the following.
    o	1 Hub VNET
        	1 Mgmt subnet, 1 GatewaySubnet, 1 AzureFirewallSubnet
     o	2 Spoke VNET
        	Each spoke has 1 workload subnet
     o	1 VPN Gateway
     o	Peerings between hub&spoke VNETs (Allow gateway transit)
     o	3 NSGs (No custom rules)
     o	1 Azure Firewall (No rules) with multiple public IP options
     o	2 UDRs (attached to the workload subnets of Spoke VNETs and Azure Firewall is set as nexthop.)

Values are defined as variables in JSON. There is prepared the parameters.json file. If you want, you can replace the variables with parameters.
