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
|L|2.5.4.7|Locality|Rapperswil|
|ST|2.5.4.8|State or Province|St. Gallen|
|street|2.5.4.9|Street Address|Oberseestrasse 10|
|O|2.5.4.10|Organization|strongSwan Project|
|OU|2.5.4.11|Organizational Unit|Research|
|T|2.5.4.12|Title|Software Engineer|
|D|2.5.4.13|Description|Main VPN gateway|
|postalAddress|2.5.4.16|Postal Address|Oberseestrasse 10 8640 Rapperswil Switzerland|
|postalCode|2.5.4.17|Postal Code|8640|
|N|2.5.4.41|Name (should not be used directly)||
|G|2.5.4.42|Given Name|John|
|I|2.5.4.43|Initials|J. T.|
|ID|2.5.4.45|Unique Identifier||
|dnQualifier|2.5.4.46|DN Qualifier (e.g. a timestamp or serial number)|20190214115113Z or 51314E|
|dmdName|2.5.4.54|DMD Name||
|pseudonym|2.5.4.65|Pseudonym||
