---
cssclass: "qs"
---
### SORT

Takes a field name and a sort order, either `asc` or `desc`

To sort the above query by most recent
```
	```dataview
	TABLE
	file.cday AS "Created on"
	FROM -#log/journal
	WHERE file.cday >= date(today) - dur(4 days)
	SORT file.cday desc
	```
```
```dataview
TABLE
file.cday AS "Created on"
FROM -#log/journal
WHERE (file.cday >= date(today) - dur(4 days))
SORT file.cday desc
LIMIT 7
```
---
up:: [[Zettelkasten Implementation in Obsidian|Implementation]]
tags:: #note/product #effort/ObsPKMClass, #note/reference #on/Obsidian #on/PKM 
prev:: [[Dataview Fields]]
next:: 
