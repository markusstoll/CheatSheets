### Hash of public key

#### Create TLSA Hash
```
openssl x509 -in <zert> -pubkey -noout | openssl pkey -pubin -outform DER | openssl sha256
```

#### TSLA Entry
```
(2|3) 1 1 <HASH>
```

### Create TLSA Hash

#### Decode a key file
```
openssl rsa -text -in <key-file>
```


####Debugging proxies for encrypted network traffic
* Fiddler
* Charlse
* burpsuite


