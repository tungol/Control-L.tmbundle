Control-L.tmbundle
------------------

Bringing form feeds to TextMate!

## Huh?

A page break, or form feed character is an ASCII whitespace character which originally signaled
a printer to advance to the next page before continuing to print the current document.
It can still be used today to break a document up into logical pages.

Representation of this character varies: 

 - `^L` (control-L) is traditional
 - `\f` is the C-style escape sequence
 - ␌ is the Unicode Control Pictures character for form feed
 - TextMate shows it as `<NP>`

## Okay, but what is this bundle specifically?

This bundle makes it easy to type ^L and move between these pages in the style
of the Emacs `forward-page` and `backward-page` functions.

The forward-page function moves the cursor to just after the next page break,
or to the end of the current document.

The backward-page function moves the cursor to just after the previous page break,
or to the beginning of the current document.

| Binding    | Action        |
|:-----------|:--------------|
| Command-^L | Insert ^L     |
| Command-^] | forward-page  |
| Command-^[ | backward-page |
