####SQL

```
merge into TABLEA ta
using
(
   select id, rownumber() AS position from TABLEA t2
    where <filter>
    order by t2.<order>
) as ta2
  ON ta.id = ta2.id
  WHEN MATCHED THEN UPDATE SET
    ta.position = ta2.position;
```


