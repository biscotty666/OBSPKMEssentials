---
cssclass: "qs"
---
### WHERE

Where allows you to apply conditions to return notes. 

To show all notes created in the last 4 days sorted by date, not including the daily notes:
```
	```dataview
	TABLE
	file.cday AS "Created on"
	FROM -#log/journal
	WHERE file.cday >= date(today) - dur(4 days)
	```
```
```dataview
TABLE
file.cday AS "Created on"
FROM -#log/journal
WHERE (file.cday >= date(today) - dur(4 days))
LIMIT 6
```

---
up:: [[Zettelkasten Implementation in Obsidian|Implementation]]
tags:: #note/product #effort/ObsPKMClass, #note/reference #on/Obsidian #on/PKM 
prev:: [[Dataview Fields]]
next:: 
