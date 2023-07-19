---
cssclass: "qs"
---
## Dates

Dates should be entered in the format `YYYY-MM-DD`. 

The tasks plugin uses icons to give meaning to dates which immediately follow the icon.

|Type|Icon|Queries|Note|
|---|---|---|---|
|Due Date|📅|`due`|Also matches `happens`|
|Scheduled Date|⏳|`scheduled`|Also matches `happens`|
|Start Date|🛫|`starts`|Also matches `happens`|
|Created Date|➕|`created`|Automatically added when using the modal|
|Done Date|✅|`done`|Automatically added when checked off|
|Recurring Date|🔁||Creates a new task when checked off|

#### Discrete dates

Absolute dates should be entered with the format "YYYY-MM-DD", eg. `2023-06-24`.

Relative dates are relative to today's date. Examples:

- `yesterday`
- `today`
- `tomorrow`
- `next monday`
- `last friday`
- `14 days ago`
- `in two weeks`
- `14 October` (the current year will be used)
- `May` (1st May in the current year will be used)

#### Date ranges

Two absolute dates in succession define an inclusive range.

Relative date ranges are defined by  `this`, `next` or `last` followed by `week`, `month`, `quarter` or `year`.

Queries use `in`, `after`, `next` or `before`.

- Can use  `is recurring` or `is not recurring`

%%

---
up:: [[Basic Task Management]]
tags:: #on/Obsidian #on/PKM  #note/product #effort/ObsPKMClass 
prev:: 
next:: 
%%