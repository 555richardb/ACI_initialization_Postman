# ACI_initialization_Postman
Initializing the ACI fabric through postman

- This project details are in WIP but I have already uploaded the postman collection export.
- More to come...

## REST API calls that covered
- APIC login
- APIC API token timeout extend
- Adding switches to fabric
- VPC protection groups
- Leaf Interface Profiles
- Leaf Switch profile + leaf switch selector
- VLAN pool
- VLAN IDs to VLAN pool
- Domains
- AAEP
- Interface policies (CDP/MCP/LLDP/Link level/STP/LACP)
- Interface policy groups
  - Single port
  - Port-channel
  - Virtual port-channel
- Leaf Interface selector to Leaf interface profile
- Enable HTTP -> HTTPS redirect
- NTP servers
- DNS servers
- DNS search domain
- BGP AS number assignment
- Route reflector assignment
- Fabric best practises 1
- Fabric best practises 2
- OOB IP assignment
- SNMP Admin
- SNMP v2 communities
- SNMP traps

# Postman Variables
|Variable | Description | Note
|---------|-------------|-------|
|{{apic}} |Hostname/IP of the APIC | Environmental variable|
|{{token}} | token from the apic login |Environmental variable|
|{{APICusername}}|Username|Environmental variable|
|{{APICpassword}}|Password|Environmental variable|
|{{NODE_SN}}|Node serial number||
|{{NODE_ID}}|Assigned Node ID||
|{{NODE_NAME}}|Hostname of the device||
|{{NODE_ROLE}}|Node role (spine/leaf)||
|{{VPC_PROT_GROUP}}|VPC protection group Name||
|{{LEAF_NODE_ID}}|VPC node ID||
|{{LEAF_NODE_1}}|VPC member 1 Leaf ID||
|{{LEAF_NODE_2}}|VPC member 2 Leaf ID||
|{{LIP_NAME}}|Leaf Interface Profile name||
TBC...
