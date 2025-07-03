# Incident: Network Down

## Description
Users lost access to the internet. Diagnosed a misconfigured gateway.



## Fix
Reconfigured default gateway on core switch.
   Switch> enable
Switch# configure terminal
Switch(config)# no ip default-gateway <old-gateway-ip>
Switch(config)# ip default-gateway <new-gateway-ip>
Switch(config)# ip default-gateway 192.168.1.1
Switch(config)# exit
Switch# write memory

