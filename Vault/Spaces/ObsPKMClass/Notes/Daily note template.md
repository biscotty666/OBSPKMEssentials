---
cssclass: "qs"
---
## Daily note template Content

Let's start with some frontmatter. Create a file Extras/Templates/Daily Note and add

```
---
date: {{date}}
tags: #log/journal #note/daily 
---
```

Then create a basic layout with headers. I've added some JavaScript at the end. I'm not going to explain it now, so just go with it 😉

Note that since we are putting these log entries on the daily note we don't need a date field for it since we can get the date from the file name.

```
## {{title}}

### Today's Goals

### Today's Progress

### Reflections

### Logs

#### Study

Study Topic:: 
Study Notes:: 

#### Home

Home Task::

---
## Yesterday's Note

<%*
const yesterday = tp.date.yesterday("YYYY-MM-DD")
tR += "![[" + [[yesterday]] + "]]"
%>

```

[[Daily Note Template Instructions]]


---

## Backmatter

up:: [[3.4 Daily Note]]
tags:: #on/Obsidian, #on/PKM, #note/product, #effort/ObsPKMClass, #note/reference
prev:: [[Daily Notes in Obsidian - Basic]]
next:: [[Daily Note Template Instructions]]
