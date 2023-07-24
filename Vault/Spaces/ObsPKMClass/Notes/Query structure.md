---
cssclass: "qs"
---
## Query structure

### Mandatory

You must start by saying whether you want a LIST, TABLE, TASK or CALENDAR. We will almost always use TABLE. 

This is the most basic query. Since this will return every note in my vault, for convenience I will go ahead and set a LIMIT for number of notes I want returned. The syntax and purpose is self-explanatory.

```
	```dataview
	TABLE
	LIMIT 3
	```
```
```dataview
TABLE
LIMIT 3
```

It will return every note in your vault (within LIMITs 😉).

You may want to see other information about your notes in the table. You can list those after TABLE.

```
TABLE
file.tags, file.etags, tags
LIMIT 3
```

```dataview
TABLE
file.tags, file.etags, tags
LIMIT 3
```
As you can see, you usually want file.etags, which is the same as just writing "tags".

In addition to fields you declare there is a lot of automatically generated (implicit) metadata for [[Dataview Implicit Fields#Pages|notes]], [[Dataview Implicit Fields#Lists and tasks|lists and tasks]].

You can change the table headers with "as"

```dataview
TABLE 
file.cday as "Created on"
LIMIT 3
```
---
up:: [[3.1 Dataview]]
tags:: #note/product #effort/ObsPKMClass, #note/reference #on/Obsidian #on/PKM 
prev:: [[Dataview Fields]]
next:: 
