# create-private-ssl-mikrotik
cara membuat private ssl mikrotik
```code
/certificate
sign myCA ca-crl-host=192.168.128.104
sign server ca=myCa name=server
sign client ca=myCa name=client 
```
set menjadi trusted
```code
/certificate
set myCA trusted=yes
set server trusted=yes
set client trusted=yes
```
export ssl ke files
```code
/certificate export-certificate myCA
/certificate export-certificate client 
```
selesai, sertifikat ssl sudah bisa digunakan!!!
