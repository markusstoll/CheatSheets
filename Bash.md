####Rename / Copy files
```
for i in *ie8.css; { cp $i  ${i%ie8.css}ie7.css; }
```

```
for i in *.mkv; { mv "$i" "${i// /_}"; }
```

