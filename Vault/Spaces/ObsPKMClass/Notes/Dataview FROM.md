---
cssclass: "qs"
---
### FROM

FROM defines the "source", or where you want to look for information. (Don't confuse this with WHERE which we use to create conditions on the notes returned.)

The source can be
- tags
- filenames
- directories
- Any arbitrary [[Dataview Fields|fields]] you create

To list all files tagged #effort/ObsPKMClass

```
	```dataview
 	TABLE file.etags as Tags
 	FROM #effort/ObsPKMClass 
 	```
```
```dataview
TABLE file.etags as Tags
FROM #effort/ObsPKMClass 
LIMIT 3
```


For all files in a certain directory
```
	```dataview
	TABLE
	file.path as Path
	FROM "Spaces/ObsPKMClass"
	LIMIT 5
```
```dataview
TABLE
file.path as Path
FROM "Spaces/ObsPKMClass"
LIMIT 5
```

As you can see it looks in sub-directories as well. We could exclude a specific sub-directory like this:

```
	```dataview
	TABLE
	file.path as Path
	FROM "Spaces/ObsPKMClass" AND -"Spaces/ObsPKMClass/Chapters"
	LIMIT 5
```
```dataview
TABLE
file.path as Path
FROM "Spaces/ObsPKMClass" AND -"Spaces/ObsPKMClass/Chapters"
LIMIT 5
```
---
up:: [[3.1 Dataview]]
tags:: #note/product #effort/ObsPKMClass, #note/reference #on/Obsidian #on/PKM 
prev:: [[Dataview Fields]]
next:: [[Dataview WHERE]]
