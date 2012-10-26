***Sip Digest Password Checker***

Checks the password for a registration message


Uses nodejs to install do

```bash

git clone http://github.com/bryanpaluch/sip-digest-checker
cd sip-digest-checker
npm install
node server.js

```
runs on port 3000, Point your browser to http://localhost:3000  or your
servers ip

***Test Case***
```bash
SIP/2.0 401 Unauthorized
From:
<sip:001DCEA4AA69001@ims.cabletown.com>;tag=4642a8-afe8a13-13c4-50029-50897e4e-1f5c90e7-50897e4e
To: <sip:001DCEA4AA69001@ims.cabletown.com>;tag=86ts16q7
Call-ID: 46c170-afe8a13-13c4-50029-50897e4e-2805f0b9-50897e4e
CSeq: 1 REGISTER
Via: SIP/2.0/UDP
10.254.138.19:5060;rport=5060;branch=z9hG4bK-50897e4e-991561ea-691d53ad
WWW-Authenticate: Digest
realm="ims.cabletown.com",nonce="0CcTlBi1d+yChEUb073szA==",algorithm=MD5
Content-Length: 0

test case

REGISTER sip:ims.cabletown.com SIP/2.0
From:
<sip:001DCEA4AA69001@ims.cabletown.com>;tag=4642a8-afe8a13-13c4-50029-50897e4e-1f5c90e7-50897e4e
To: <sip:001DCEA4AA69001@ims.cabletown.com>
Call-ID: 46c170-afe8a13-13c4-50029-50897e4e-2805f0b9-50897e4e
CSeq: 2 REGISTER
Via: SIP/2.0/UDP
10.254.138.19:5060;branch=z9hG4bK-50897e4e-9915633e-2cc92bf0
Max-Forwards: 70
Supported: timer,replaces,join,tdialog,100rel,histinfo,path
Authorization: Digest
username="001DCEA4AA6901",realm="ims.cabletown.com",nonce="0CcTlBi1d+yChEUb073szA==",uri="sip:ims.cabletown.com",response="fac665b601d8df845a16d6729b9a5a3f",algorithm=MD5
Contact: <sip:001DCEA4AA69001@10.254.138.19:5060>;expires=3600
Allow: INVITE,ACK,BYE,CANCEL,NOTIFY,PRACK,UPDATE,OPTIONS
Content-Length: 0

username: 001DCEA4AA6901
password : mQCbMv1KzrR1NFkWrm1IvO1aMJrw/LKjlkEXlcz9msE



