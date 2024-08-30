# Access Control Lists
## Standard (Numbered)
* To create a numbered standard access control list, use the following global configuration command:
  * `access-list <access-list-number> {deny | permit | remark text} <source> [source-wildcard] [log]
    * access-list-number - This is the decimal number of the ACL; Standard ACL number range is 1 to 99 or 1300 to 1999.
    * deny or permit or remark:
      * Deny -> denies access if the condition is matched
      * Permit -> Permits access if the condition is matched
      * Remark *text* -> Optional; Adds a text entry for documentation purposes. Is limited to 100 characters per remark.
    * *source* - This identifies the source network or host address to filter; use the `any` keyword to specify all networks; use the <host ip-address> keyword or simply enter an <ip-address> (without the host keyword) to identify a specific IP address.
    * *source-wildcard* - Optional; A 32-bit wildcard mask that is applied to the source.
    * *log* - Optional; This keyword generates and sends an informational message whenever the ACE is matched. This message includes ACL number, matched condition (i.e., permitted or denied), source address, and number of packets. This message is generated for the first matched packet. This keyword should only be implemented for troubleshooting or security reasons.

## Extended (Numbered)
* Create a numbered extended access control list:
  * `access-list <access-list-number> {deny | permit | remark text} <protocol> <source> <source-wildcard> [operator {port}] <destination> <destination-wildcard> [operator {port}] [established] [log]`
    * *access-list-number* - This is the decimal number of the access control list
    * deny or permit or remark:
      * Deny -> denies access if the condition is matched
      * Permit -> Permits access if the condition is matched
      * Remark *text* -> Optional; Adds a text entry for documentation purposes. Is limited to 100 characters per remark.
    * *protocol* - Name or number of an internet protocol; common keywords include ip, tcp, udp and icmp. For example, the `ip` keyword matches all IP protocols.
    * *source* - This identifies the source network or host address to filter; use the `any` keyword to specify all networks; use the <host ip-address> keyword or simply enter an <ip-address> (without the host keyword) to identify a specific IP address.
    * *source-wildcard* - Optional; A 32-bit wildcard mask that is applied to the source.
    * *destination* - This identifies the destination network or host address to filter; use the `any` keyword to specify all networks; use the `host ip-address` keyword or `ip-address`.
    * *destination-wildcard* - Optional; This is a 32-bit wildcard mask that is applied to the destination.
    * *operator* - Optional; This compares source or destination ports. Some operators include `lt` (less than), `gt` (greater than), `eq` (equal), and `neq` (not equal).
    * *port* - Optional; The decimal number or name of a TCP or UDP port.
    * *established* - Optional; For the TCP protocol only. This is a 1st generation firewall feature.
    * *log* - Optional; This keyword generates and sends an informational message whenever the ACE is matched. This message includes ACL number, matched condition (i.e., permitted or denied), source address, and number of packets. This message is generated for the first matched packet. This keyword should only be implemented for troubleshooting or security reasons.

## Other
* To apply an IPv4 access control list to an interface once it has been created:
  * ip access-group {access-list-number `or` access-list-name} {in `or` out}
*  To remove an access control list from an interface, first enter the `no ip access-group` interface configuration command.
*  To remove the access control list entirely, use the `no access-list` global configuration command.
