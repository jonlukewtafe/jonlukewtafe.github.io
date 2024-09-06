# Network Subnetting
## Calculating a Subnet Mask from an IP Address with CIDR Notation
1. Convert the CIDR notation to binary
    1. A /24 CIDR becomes 11111111.11111111.11111111.00000000
    2. A /25 CIDR becomes 11111111.11111111.11111111.10000000
    3. a /30 CIDR becomes 11111111.11111111.11111111.11111100
2. Once in binary, calculate the total binary values of each octet:
    1. This can be achieved by adding up the decimal values for each of the bits based on the ruler outlined below.
        1. A /24 CIDR with a binary value of 11111111.11111111.11111111.00000000 has a subnet mask of 255.255.255.0
        2. A /25 CIDR with a binary value of 11111111.11111111.11111111.10000000 has a subnet mask of 255.255.255.128
        3. A /30 CIDR with a binary value of 11111111.11111111.11111111.11111100 has a subnet mask of 255.255.255.252
### Subnet Ruler
Each binary octet (8 bits) below will use the following values from left to right to determine the total decimal value of the octet: `128-64-32-16-8-4-2-1` 

## Calculating the Wildcard Mask using the Subnet Mask
1. For each octet in the subnet mask, subtract the decimal value from 255.
    1. The wildcard mask for the /24 subnet mask (255.255.255.0) is 0.0.0.255
    2. The wildcard mask for the /30 subnet mask (255.255.255.252) is 0.0.0.3
