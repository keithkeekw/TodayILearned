# Deleting Words in Vim

|Command|Description|
|:---|:-----|
|x|Delete the current character.|
|dw|Delete the current word.|
|dd|Delete the current line.|
|5dd|Delete five(5) lines.|
|d$|Delete till the end of line.|
|d0|Delete till the beginning of the line|
|dt<char>| Delete toi the character from the cursor.|
|:1,.d|Delete to the beginning of the file. Delete from line 1 to the current line position.|
|:., $d|Delete to the end of the file. From the current position to end of the file, delete.|
|D|Delete till end of the line|
|I|Move cursor to the beginning of the line and turn on `Insert` mode.|
|A|Move cursor to the end of the line and turn on `Insert` mode.|
|daw| To delete a word from any position of the cursor within the word. It will delete any trailing whitespace too.|
|diw| To delete a word from any position of the cursor within the word. It will **NOT** delete any trailing whitespace too.|
|dap|Delete the entire paragraph.|
|das|Delete the sentence.|

---
### Source
[AlvinAlexander.com](https://alvinalexander.com/linux/vi-vim-delete-line-commands-to-end/)
