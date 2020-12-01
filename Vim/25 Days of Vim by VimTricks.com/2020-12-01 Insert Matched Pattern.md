# Insert Matched Pattern

```
%s/https\?.*/[&](&)/g
```

Here's what this does:
- `%` – set the range to the entire file
- `%s` – substitution
- `%/https\?.*/`– regex to match http or https and anything else after it
- `[&](&)`– The & is the magic here and inserts the matched text. In this case, the URL. The rest of the characters are interpreted literally, giving us the linked URL in the resulting markdown.
- `/g` changes all the matches on a line

**Video:** [Click Here](/resources/use-match.mp4)

**Source:** [VimTricks.com](https://vimtricks.com/p/vimtrick-insert-matched-pattern/)
