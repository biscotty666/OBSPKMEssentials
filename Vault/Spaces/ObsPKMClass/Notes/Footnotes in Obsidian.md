---
cssclass: "qs"
aliases: Footnotes
---
#### Footnotes in Obsidian

Footnotes can be declared by putting a caret and a number in square brackets, eg.  `[^1]` after some text. Somewhere (anywhere) else in the note you declare the content of the footnote with `[^1]:`.

I would like to give this text a reference[^1]. And here[^2] is another.

```
This is typed in the note but invisible in Read View
[^1]:The content of the first reference
```

[^1]:The content of the first reference

You can add the contents of the reference in-line as well with `^[some reference information]`

In this case I'll just make a citation^[This is the in-line citation] in-line.

```
This is typed in the note but invisible in Read View
[^2]: The second citation we made earlier.
```

[^2]: The second citation we made earlier.

Notice that, in Read View, Obsidian automatically adjusts the numbering order of the footnotes to be sequential regardless of the order or numbers you type in the note.

Footnotes can contain links, formatting and back-links, as you can see from this quote from an earlier note[^3], although it doesn't seem to align properly when you have external links.

```
This is typed in the note but invisible in Read View
[^3]: Halasz, Frank G. (July 1988). ["Reflections on NoteCards: Seven Issues for the Next Generation of Hypermedia Systems"](https://doi.org/10.1145%2F48511.48514). _[Communications of the ACM](https://en.wikipedia.org/wiki/Communications_of_the_ACM "Communications of the ACM")_. **31** (7): 836–852. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1145/48511.48514](https://doi.org/10.1145%2F48511.48514).
```

[^3]: Halasz, Frank G. (July 1988). ["Reflections on NoteCards: Seven Issues for the Next Generation of Hypermedia Systems"](https://doi.org/10.1145%2F48511.48514). _[Communications of the ACM](https://en.wikipedia.org/wiki/Communications_of_the_ACM "Communications of the ACM")_. **31** (7): 836–852. [doi](https://en.wikipedia.org/wiki/Doi_(identifier) "Doi (identifier)"):[10.1145/48511.48514](https://doi.org/10.1145%2F48511.48514).


%%

---
up:: [[2.1 Markdown]]
tags:: #on/Obsidian #on/PKM  #note/product #effort/ObsPKMClass 
prev:: [[Codeblocks]]
next:: [[Tags]]
%%
