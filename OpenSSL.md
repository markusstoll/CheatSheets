####Decode a Certificate
```
openssl x509 -text -in <cert-file>
```

####Decode a Certificate request
```
openssl asn1parse -in <csr-file>
```

####Decode a key file
```
openssl rsa -text -in <key-file>
```

####Manual https input
```
(echo -ne "GET / HTTP/1.0\r\nHost: <hostname>\r\n\r\n"; cat) | openssl s_client -connect <hostname>:443 -servername <hostname>
```

####Check passwd hash (e. g. from /etc/shadow)
```
(echo -ne "GET / HTTP/1.0\r\nHost: <hostname>\r\n\r\n"; cat) | openssl s_client -connect <hostname>:443 -servername <hostname>
```

####Debugging proxies for encrypted network traffic
* Fiddler
* Charlse
* burpsuite


