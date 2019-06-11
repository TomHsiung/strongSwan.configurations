# strongSwan.configurations
Basic strongSwan server end configurations for Apple devices

# Function
Set up a client-server mode IPsec connection.

# Parameter interpretation
Refer the official website of storngSwan for more information.

# Contents
1) ipsec.conf.roadwarrior file is the most simple configration for roadwarrior mode. 
2) ipsec.conf.roadwarrior.certificate.mode is the configration for roadwarrior mode, but additionaly to authorize clients via certificates. 
3) Other mode is to be update in future.

# Diffie-Hellman Groups
|Diffie-Hellman Group Number|Diffie-Hellman Group Name|RFC|Predefined|
| - | - | - | - |
|Group 1 |768-bit modulus MODP Group                           |RFC 7296|Yes|
|Group 2 |1024-bit modulus MODP Group                          |RFC 7296|Yes|
|Group 5 |1536-bit modulus MODP Group                          |RFC 3526|Yes|
|Group 14|2048-bit modulus MODP Group                          |RFC 3526|Yes|
|Group 15|3072-bit modulus MODP Group                          |RFC 3526|No |
|Group 16|4096-bit modulus MODP Group                          |RFC 3526|No |
|Group 17|6144-bit modulus MODP Group                          |RFC 3526|No |
|Group 18|8192-bit modulus MODP Group                          |RFC 3526|No |
|Group 19|256-bit random Elliptic Curve Group                  |RFC 5903|Yes|
|Group 20|384-bit random Elliptic Curve Group                  |RFC 5903|Yes|
|Group 24|2048-bit MODP Group with 256-bit Prime Order Subgroup|RFC 5114|No |

# Supported RDN Types
|Identifier|OID|Description|Example|
| - | - | - | - |
|CN|2.5.4.3|Common Name|vpn.strongswan.org or John Smith|
|S|2.5.4.4|Surname|Smith|
|SN|2.5.4.5|Serial Number|ZX52376|
|C|2.5.4.6|Country (ISO 3166 two-letter code)|CH|
