#### Obsidian Templates

NB. in a later part of this course we will look at a plugin called Templater. For now we'll stick with the native Template functionality.

##### Importance of templates
- Provide a pre-defined structure for similar notes
- Imported with Ctrl-T
- Enforce consistency
	- tags
	- backlinks
- Prompt for other metadata
- Makes you much faster and more efficient

##### Using templates
1. Create a directory `Extras/Templates`.
2. In Settings/Templates enter the new directory. You can also change the date format if you like. For example `dddd, MMMM Mo` would display as "Saturday, January 11th".
3. Notes in this directory can be pasted into a document with the "Insert Template" command (Ctrl-T).
4. Used for Daily Notes and Fleeting Notes
5. Whenever you are taking a series of notes with similar metadata

##### Create a template for fleeting notes

We only need a simple template for these notes. We'll have the template show the filename, add a `#note/new` tag, and add a section for a reference
1. Create a new note called Fleeting Note
2. Copy the following into the note
```
### {{title}}
#note/new 

---

#### References

```
3. Place the note in the `Extras/Templates` directory
4. Create a new note, hit Ctrl-T and select the Fleeting Note template

---
up:: [[Zettelkasten Implementation in Obsidian|Implementation]]
tags:: #note/product #effort/ObsPKMClass, #note/reference #on/Obsidian #on/PKM 
prev:: [[Other considerations making notes in Obsidian]]
next:: [[Obsidian Folders|Folders]]
