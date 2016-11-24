####SQL

```
merge into TABLEA t
using
(
   select id, rownumber() over() AS position from "KUNITAUSER"."K_UNTERANLIEGEN" uat where uat.anliegenid = 17 order by uat.angezeigtername
) as ua2
  ON ua.id = ua2.id
  WHEN MATCHED THEN UPDATE SET
    ua.position = ua2.position;
```


