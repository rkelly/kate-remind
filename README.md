# kate-remind

A Kate (KDE Advanced Text Editor) syntax highlighting definition for the [Remind](https://www.roaringpenguin.com/products/remind) scripting language

Remind is a scripting language-driven reminder program for *nix systems licensed under the GPL.

[remind.vim](http://www.vim.org/scripts/script.php?script_id=1536) has been available since 2006 for Vim users. This is a definition file for Kate users. It makes entry of reminders via Kate more enjoyable, and increases accuracy. Before using sytax coloring, I would often forget the `MSG` keyword. With syntax coloring, mistakes like this are visually obvious.

This definition seeks to:

- highlight common entry errors
- give prominence to the content (the date, time and message body), not the keywords
- use the user-specified color palette

## Screenshots

### Before

![](https://raw.githubusercontent.com/rkelly/kate-remind/master/before.png "Before syntax coloring")

### After

![](https://raw.githubusercontent.com/rkelly/kate-remind/master/after.png "After syntax coloring")

## Installation

### katepart5/Linux

```bash
mkdir -p ~/.local/share/katepart5/syntax
wget https://raw.githubusercontent.com/rkelly/kate-remind/master/remind.xml \
    -O ~/.local/share/katepart5/syntax/remind.xml
```

### Other Kate Versions/Linux Distros

Other versions of Kate, or other Linux distributions may require you to save the [syntax.xml file](https://raw.githubusercontent.com/rkelly/kate-remind/master/remind.xml) instead to one of the following locations:

#### Linux

- `~/.kde/share/apps/katepart/syntax`
- `/usr/share/kde4/apps/katepart/syntax`

#### Windows

- `%USERPROFILE%\AppData\Local\katepart5\syntax`

Sometimes the `syntax` directory may not exist, and will have to be created. After installing the file, *Kate must be restarted* before it will read it.

After installation, Remind syntax highlighting will automatically start when opening a `*.rem` or `*.remind` file. It can also be set manually in the bottom right corner of the Kate window. The Remind syntax is filed in the Scripts folder.

## Status

This definition is usable as-is, but is by no means complete. Contributions are welcome.
