### Check DNSSEC
Openssl 1.1 required

```
dig . DNSKEY | grep -Ev '^($|;)' > root.keys


```

