# create-private-ssl-mikrotik
cara membuat private ssl mikrotik
```code
/certificate
sign CA ca-crl-host=192.168.128.104
sign Server ca=myCa name=server
sign Client ca=myCa name=client 
```
