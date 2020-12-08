### Windows CMD 

#### Delete files older than 1 day
```
 forfiles /p "D:\Temp\" /s /m *.* /D -1 /C "cmd /c del @path"
 ```

