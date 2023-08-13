# Cisco Inital Router Configuration Commands
|Description|Command|
| -- | -- |
|User EXEC mode |Router > |
|Enter the privileged EXEC mode |Router > **enable** <br></br> Router # |
|Enter the global configuration mode.  |**configure terminal**  <br></br>Example:  <br></br>Router# **configure terminal**  <br></br>Router(config)#|
|Specify the name for the router.  |**hostname** *name*  <br></br>Example:  <br></br>Router(config)# **hostname Router1**  <br></br>Router1(config)#|
|Disable DNS lookup |Router(config)# **no ip domain-lookup** |
|Specify an encrypted password to prevent unauthorized access to the privileged exec mode.  |**enable secret** *password*  <br></br>Example:  <br></br>Router(config)# **enable secret cisco**  <br></br>Router(config)#|
|Specify a password to prevent unauthorized access to the console.  |**line con 0**  **password** *password*  **login**  <br></br>Example:  <br></br>Router(config)# **line con 0**  <br></br>Router(config-line)# **password class**  <br></br>Router(config-line)# **login**  <br></br>Router(config)#|
|Specify a password to prevent unauthorized telnet access.  <br></br>Router vty lines: 0 15  <br></br>Switch vty lines: 0 15  <br></br>|**line vty 0 4**  **password** *password*  **login**  <br></br>Example:  <br></br>Router(config)# **line vty 0 4**  <br></br>Router(config-line)# **password class**  <br></br>Router(config-line)# **login**  <br></br>Router(config-line)#|
|Encrypt the plaintext passwords |**service password-encryption** |
|Configure the MOTD banner.  |**Banner motd %** *message* **%** <br></br>Example:  <br></br>Router(config)# **banner motd % Welcome %** <br></br>Router(config)#|
|Configure an interface.  <br></br>Router- interface is OFF by default  <br></br>Switch- interface is ON by default  <br></br>|Router(config)# **interface fa0/0**  <br></br>Router(config-if)# **description** *description*  <br></br>Router(config-if)# **ip address** *address mask*  <br></br>Router(config-if)# **no shutdown**  <br></br>Router(config-if)#|
|Configure an interface IPv6 |Router(config-if)# **ipv6 address** *ipv6address/prefix* <br></br>Router(config-if)# **ipv6 address** *ipv6address* **linklocal**|
|Configure an interface.  (Gigabit interface) |Router(config)# **interface gig0/0**  <br></br>Router(config-if)# **description** *description*  <br></br>Router(config-if)# **ip address** *address mask*  <br></br>Router(config-if)# **no shutdown**|
|To enable IPv6 routing |Router(config)# **ipv6 unicast-routing**|
|Save the configuration to NVRAM.  |**copy running-config startup-config**  <br></br>Example:  <br></br>Router# **copy running-config startup-config**  Router#|
