---
cssclass: "qs"
---
## Yard Activity

### Today

```dataview
TABLE without id
species as Species, date as Date, image as Picture, notes as Notes
FROM #note/observation AND -"Extras/Templates"
WHERE date = date(today)
```

### This week

```dataview
table without id
species as Species, date as Date, image as Picture, notes as Notes
FROM #note/observation AND -"Extras/Templates"
WHERE date >= date(today) - dur(7 days)
```

### This month

```dataview
table without id
species as Species, date as Date, image as Picture, notes as Notes
from #note/observation AND -"Extras/Templates"
WHERE date >= date(today) - dur(1 month)
```

### This year

```dataview
table without id
species as Species, date as Date, image as Picture, notes as Notes
from #note/observation AND -"Extras/Templates"
WHERE date >= date(today) - dur(1 year)
```

### This month last year

```dataview
table without id
species as Species, date as Date, image as Picture, notes as Notes
from #note/observation AND -"Extras/Templates"
WHERE (date <= date(today) - dur(1 year)) AND (date >= date(today) - dur(13 months))
```

### Last year

```dataview
table without id
species as Species, date as Date, image as Picture, notes as Notes
from #note/observation AND -"Extras/Templates"
WHERE date >= date(today) - dur(2 years) AND date <= date(today) - dur(1 year)
```

### All activity

```dataview
table without id
species as Species, date as Date, image as Picture, notes as Notes
from #note/observation AND -"Extras/Templates"
WHERE file.cday >= date(today) - dur(7 days)
```
