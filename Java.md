#### Dump Heap on out of memory
```
for i in *ie8.css; { cp $i  ${i%ie8.css}ie7.css; }
```

```
for i in *.mkv; { mv "$i" "${i// /_}"; }
```

#### Find all file types
```
find . -type f | awk -F. '!a[$NF]++{print $NF}'
```


