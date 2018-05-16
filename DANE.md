#### Create TLSA Hash
```
openssl x509 -in <zert> -pubkey -noout | openssl pkey -pubin -outform DER | openssl sha256
```

#### Decode a Certificate request
```
openssl asn1parse -in <csr-file>
```

####Decode a key file
```
openssl rsa -text -in <key-file>
```


####Debugging proxies for encrypted network traffic
* Fiddler
* Charlse
* burpsuite


