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
|Group 1|:768-bit modulus MODP Group:|:RFC 7296:|Yes|
| 表格      | 第一列     | 第二列     |
| ---------- | :-----------:  | :-----------: |
| 第一行     | 第一列     | 第二列     |
