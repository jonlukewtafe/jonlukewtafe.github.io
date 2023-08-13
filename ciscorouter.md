# Cisco Inital Router Configuration Commands
|Description|Command|
| :- | :- |
|User EXEC mode |Router > |
|Enter the privileged EXEC mode |Router > **enable** <br> Router # |
|Enter the global configuration mode.  |**configure terminal**  <br>Example:  <br>Router# **configure terminal**  <br>Router(config)#  <br>|
|Specify the name for the router.  |**hostname** *name*  <br>Example:  <br>Router(config)# **hostname Router1**  <br>Router1(config)#  <br>|
|Disable DNS lookup |Router(config)# **no ip domain-lookup** |
|Specify an encrypted password to prevent unauthorized access to the privileged exec mode.  |**enable secret** *password*  <br>Example:  <br>Router(config)# **enable secret cisco**  <br>Router(config)#  <br>|
|Specify a password to prevent unauthorized access to the console.  |**line con 0**  **password** *password*  **login**  <br>Example:  <br>Router(config)# **line con 0**  <br>Router(config-line)# **password class**  <br>Router(config-line)# **login**  <br>Router(config)#  <br>|
|Specify a password to prevent unauthorized telnet access.  <br>Router vty lines: 0 15  <br>Switch vty lines: 0 15  <br>|**line vty 0 4**  **password** *password*  **login**  <br>Example:  <br>Router(config)# **line vty 0 4**  <br>Router(config-line)# **password class**  <br>Router(config-line)# **login**  <br>Router(config-line)#  <br>|
|Encrypt the plaintext passwords |**service password-encryption** |
|Configure the MOTD banner.  |**Banner motd %** *message* **%** <br>Example:  <br>Router(config)# **banner motd % Welcome %** <br>Router(config)#  <br>|
|Configure an interface.  <br>Router- interface is OFF by default  <br>Switch- interface is ON by default  <br>|Router(config)# **interface fa0/0**  <br>Router(config-if)# **description** *description*  <br>Router(config-if)# **ip address** *address mask*  <br>Router(config-if)# **no shutdown**  <br>Router(config-if)#  <br>|
|Configure an interface IPv6 |Router(config-if)# **ipv6 address** *ipv6address/prefix* <br>Router(config-if)# **ipv6 address** *ipv6address* **linklocal** <br>|
|Configure an interface.  (Gigabit interface) |Router(config)# **interface gig0/0**  <br>Router(config-if)# **description** *description*  <br>Router(config-if)# **ip address** *address mask*  <br>Router(config-if)# **no shutdown** <br>|
|To enable IPv6 routing |Router(config)# **ipv6 unicast-routing** |
|Save the configuration to NVRAM.  |**copy running-config startup-config**  <br>Example:  <br>Router# **copy running-config startup-config**  Router#  <br>|
