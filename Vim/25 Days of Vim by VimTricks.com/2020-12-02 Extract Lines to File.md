# Extract Lines to File

- `shift-v` to visually select some lines
- `:w` path/to/new/file.rb<Enter> to save those lines to a new file
- `gv` to reselect the last visual selection
- `d` to delete that selection

Another variation on this is to use >> before your filename to append rather than overwrite.

- `:w >>path/to/new/file.rb<Enter>` appends the lines to the existing file  

**Source:** [VimTricks.com](https://vimtricks.com/p/vimtrick-extract-lines-to-file/)
