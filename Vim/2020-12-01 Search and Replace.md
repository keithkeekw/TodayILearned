# Vim Search and Replace

**Original Text**
Does a boy get a chance to paint black a fence every day? That put the thing in a new light. Ben Rogers stopped nibbling his apple. Tom swept his brush daintily back and forth–stepped back to note the effect–added a touch here and there–criticised the effect again–Ben watching every move and getting more and more interested, more and more absorbed.  

|Command|Description|
|:---|:---|
|**:s/black/white/**|Replace the first occurrence of the string ‘black’ by ‘white’|
|**:s/Ben\( Rogers\)\@!/Ben Rogers/g**|Replace every occurrence of the string ‘Ben’ by ‘Ben Rogers’ except when ‘ Rogers’ was already present|
|**:s/.*/<p>\r&\r<\/p>/**|Wrap the line between <p> and </p>|
|**:-1s/–/\&mdash;/g**| Replace every occurrence of the string ‘–‘ by ‘&mdash;’ in the preceding line|


