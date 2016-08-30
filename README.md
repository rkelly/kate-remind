# kate-remind

A Kate (KDE Advanced Text Editor) syntax highlighting definition for the [Remind](https://www.roaringpenguin.com/products/remind) scripting language

Remind is a scripting language-driven reminder program for *nix systems licensed under the GPL.

[remind.vim](http://www.vim.org/scripts/script.php?script_id=1536) has been available since 2006 for Vim users. This is a definition file for Kate users. It makes entry of reminders via Kate more enjoyable, and increases accuracy. Before using sytax coloring, I would often forget the `MSG` keyword. With syntax coloring, mistakes like this are visually obvious.

## Screenshots

### Before

![](https://raw.githubusercontent.com/rkelly/kate-remind/master/before.png "Before syntax coloring")

### After

![](https://raw.githubusercontent.com/rkelly/kate-remind/master/after.png "After syntax coloring")

## Installation

```bash
mkdir -p ~/.local/share/katepart5/syntax
wget https://raw.githubusercontent.com/rkelly/kate-remind/master/remind.xml \
    -O ~/.local/share/katepart5/syntax/remind.xml
```

## Status

This definition is usable as-is, but is by no means complete. Contributions are welcome.
