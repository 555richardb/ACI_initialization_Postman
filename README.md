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
|{{SW_PROF_NAME}}|Leaf switch Porofile name||
|{{LEAF_NODE_1}}|Leaf Node ID|should be the same as LEAF_NODE_2|
|{{LEAF_NODE_2}}|Leaf Node ID|should be the same as LEAF_NODE_1|
|{{NPSB}}|some kind of a random value|TBC|
|{{LEAF_SEL_NAME}}|Leaf Selector name||
|{{CDPMCPIPTYPE}}|CDP or MCP interface policy setting|either cdpIfP or mcpIfP |
|{{CDPMCPIPTYPE2}}|CDP or MCP interface policy setting|either cdpIfPol or mcpIfPol |
|{{CDPMCPIPNAME}}|CDP or MCP Interface policy name|
|{{CDPMCPIPSTATE1}}|CDP or MCP Interface policy state|enabled or disabled|
|{{LLDPIPTYPE}}||lldpIfP|
|{{LLDPIPTYPE2}}||lldpIfPol|
|{{LLDPIPNAME}}|LLDP interface policy name||
|{{LLDPIPSTATE1}}|lldp transmit state|enabled or disabled|
|{{LLDPIPSTATE2}}|lldp transmit state|enabled or disabled|
|{{LACPIPTYPE}}||lacplagp|
|{{LACPIPTYPE2}}||lacpLagPol|
|{{LACPIPNAME}}|LACP interface policy name||
|{{LACPIPSTATE1}}||On or LACP Active|
|{{STPIPTYPE}}||ifPol|
|{{STPIPTYPE2}}||stpIfPol|
|{{STPIPNAME}}|STP policy name||
|{{STPIPSTATE1}}||bpdu-filter,bpdu-guard|
|{{LLPIPTYPE}}||hintfpol|
|{{LLPIPTYPE2}}||fabricHIfPol|
|{{LLPIPNAME}}|Link Level policy name||
|{{LLPIPSTATE1}}|auto negotiation|on or off|
|{{LLPIPSTATE2}}|speed|100M,1G,10G,40G,inherit|
|{{LIP_NAME}}|Leaf interface profile name||
|{{IF_SEL_DESC}}|Interface selector description||
|{{IS_PORT_A}}|interface selector port A|range min|
|{{IS_PORT_B}}|interface selector port A|range max|
|{{IF_SEL_NAME}}|interface selector name||
|{{IPG_NAME}}|interface policy group||
|{{VPOOL}}|vlan pool name||
|{{VPOOLDESC}}|vlan pool||
|{{VPOOLMODE}}|vlan pool mode|static or dynamic|
|{{VLANFROM}}|vlan from |range|
|{{VLANTO}}|vlan to|range|
|{{DOMNAME}}|ACI Domain name||
|{{DOMTYPE}}|domain type|l3dom, phys, l2dom|
|{{DOMTYPE2}}||l3extDomP, physDomP,l2extDomP|
|{{AAEP}}|AAEP name||
|{{NTP_SRV}}|ntp server|IP|
|{{NTP_PREF}}||true,false|
|{{DNS_SRV}}|dns server |IP|
|{{DNS_PREF}}||true,false|
|{{DNS_DOMAIN}}|domain name||
|{{DOM_DEFAULT}}|default|true,false|
|{{AS_NUM}}|AS number||
|{{RR_NODE}}|RR node IDs||
|{{OOB_NODE_ID| node IDs for oob IP||
|{{OOB_NODE_IP}}|OOB IP||
|{{OOB_GW}}|OOB gateway||
|{{SNMPv2COM}}|SNMP community||
|{{SNMPTRAP}}|snmp trap receiver|IP|
