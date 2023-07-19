---
cssclass: "qs"
---
## Keeping logs with dataview

### Motivation

Pull together what we've learned by implementing a logging system.

### Scenario

I'm interested in the animal activity in my yard. I'd like to keep track of the birds that I see and learn more about them.

### Implementation

Our implementation will consist of:

#### An observation template

```
## {{title}}

Date:: <% tp.date.now("YYYY-MM-DD") %>
Time:: <% tp.date.now("hh:mm a") %>
Species:: [[Unknown Species]]
Description:: 
Notes:: 
Image:: 
Tags:: #note/observation 
```

#### A Map of Content

We can display observations over different time periods, eg.

```
### Today

```dataview
TABLE without id
species as Species, date as Date, image as Picture, notes as Notes
FROM #note/observation AND -"Extras/Templates"
WHERE date = date(today)
```

```
### Month

```dataview
table without id
species as Species, date as Date, image as Picture, notes as Notes
from #note/observation AND -"Extras/Templates"
WHERE date >= date(today) - dur(1 month)
```

```
### This month last year

```dataview
table without id
species as Species, date as Date, image as Picture, notes as Notes
from #note/observation AND -"Extras/Templates"
WHERE (date <= date(today) - dur(1 year)) AND (date >= date(today) - dur(13 months))
```

#### An evergreen/permanent note

For species of interest I may develop content and can draw on my observations with queries such as:

```
### Notable observations

```dataview
table without id
date as Date, image as Picture, description as Description, notes as Notes
from #note/observation 
where species = [[Rufous Hummingbird]] AND notes
```

```
### All observations

```dataview
table without id
date as Date, image as Picture, description as Description, notes as Notes
from #note/observation 
where species = [[Rufous Hummingbird]]
```


---
up:: [[ObsPKMEssentials]]
tags:: #on/Obsidian #on/PKM  #note/product #effort/ObsPKMClass 
prev:: 
next:: 