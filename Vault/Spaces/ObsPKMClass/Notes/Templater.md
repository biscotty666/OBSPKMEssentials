---
cssclass: "qsol"
---
## Templater

Templater is a **community plugin** which is used to insert "variable" information into a note. Examples would be:
- Current date or dates related to the current date
- Information about the note such as 
	- name (title)
	- created and modified date
	- tags
	- content
- Information from the frontmatter

As the name suggests, Templater is primarily used in templates.

### Setting up Templater

1. Install and activate the Templater plugin
2. Create a directory for your templates (Extras/Templates for us)
3. In the settings for Templater enter the name of your templates directory

### Inserting templates

Templater is used by placing a _template_ in a note. Templates take this form:
```
<% tp.SomeCommand %>
```

So, for example, to insert today's date I would use:

<% tp.date.now("MMM Do, YYYY") %>

To get the date the file is created on I would:

<% tp.file.creation_date("YYYY-MM-DD") %>

As you can see you need to specify the [date format](https://momentjs.com/docs/#/displaying/format/)

### Replacing templates

Once you have placed a template in a note, you can run the command `Templater: Replace Templates in the Active File` or press "Alt-R"

---
[[Obsidian Templater|Templater Reference]]

---
```todoist
name: ""
filter: "search: Templater Note"
```

---
up:: [[ObsPKMEssentials]]
tags:: #on/Obsidian #on/PKM  #note/product #effort/ObsPKMClass 
prev:: 
next:: 