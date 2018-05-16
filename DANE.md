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
```
openssl x509 -in <Zertifikatsdatei> -outform DER | openssl <sha256|sha512
```

#### TSLA Entry
```
(2|3) 0 1 <HASH>
```

### TSLA Docs

see https://www.core-networks.de/faq/tlsa-record.html

TLSA record gen:
https://www.huque.com/bin/gen_tlsa
  


