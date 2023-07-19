---
Field FM: A frontmatter field
aliases: Inline Fields, In-line Fields
---
#### Declaring fields in Obsidian

Fields can be declared _in-line_ or in [[Obsidian Frontmatter|frontmatter]].

Aliases cannot be declared in-line. All other fields seem to work in-line. The choice of how to declare these fields is just personal preference. You can decide based on the situation which way is best.

==When referring to a field in a query substitute a dash for spaces and use only lowercase.==

##### Examples
Field IL:: An in-line field
[Field BR:: An in-line field with brackets]
(Field PR:: An in-line field with parentheses)
Placed in comments nothing is visible in read mode
%%
Field COM:: A field in comments
%%

> [!example] Frontmatter
> ```dataview
> table field-fm
> where field-fm
> ```

> [!example] In-line
> ```dataview
> table field-il
> where field-il
> ```

> [!example] In-line with brackets
> ```dataview
> table field-br
> where field-br
> ```

> [!example] In-line with parenttheses
> ```dataview
> table field-pr
> where field-pr
> ```

> [!example] In-line with comments
> ```dataview
> table field-com
> where field-com
> ```



---
up:: [[Zettelkasten Implementation in Obsidian|Implementation]]
tags:: #note/product #effort/ObsPKMClass, #note/reference #on/Obsidian #on/PKM 
prev:: [[Dataview]]
next:: [[Dataview Queries]]
aliases:: Another inline