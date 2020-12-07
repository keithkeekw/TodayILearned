# Operate until Pattern

|Verb|Description|
|:---:|:---|
|d|Delete|
|c|Change|
|y|Yank|

|Motion|Description|
|:---:|:---|
|t|Un**t**ill|

Examples:
- `dtX`: Delete everything until the first `X`. `X` can be any character.
- `ctX`: Change everything until the first `X`. `X` can be any character. That is, deletes and leaves you in insert mode.
- `ytX`: Yanks(copies) everything until the first `X`. 

Can use **patterns** as well. Below are a few examples:
- `d/foo<Enter>`: Delete until `foo` is found.
- `c/bar<Enter>`: Change everything up until `bar`
- `y/pattern<Enter>`: Yang everything up until `pattern`

**Source:**[VimTricks.com](https://vimtricks.com/p/vimtrick-operate-until-pattern/)
