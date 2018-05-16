### Check DNSSEC
Openssl 1.1 required

```
dig . DNSKEY | grep -Ev '^($|;)' > root.keys

dig +sigchase +trusted-key=./root.keys www.eurid.eu. A | cat -n

```

