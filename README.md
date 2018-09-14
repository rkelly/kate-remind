# kate-remind

A Kate (KDE Advanced Text Editor) syntax highlighting definition for the [Remind](https://www.roaringpenguin.com/products/remind) scripting language

Remind is a scripting language-driven reminder program for *nix systems licensed under the GPL.

[remind.vim](http://www.vim.org/scripts/script.php?script_id=1536) has been available since 2006 for Vim users. This is a definition file for Kate users. It makes entry of reminders via Kate more enjoyable, and increases accuracy. Before using sytax coloring, I would often forget the `MSG` keyword. With syntax coloring, mistakes like this are visually obvious.

Key goals for this definition are to:

- highlight common entry errors
- encourage the reader to focus on the content (the date, time and message body), not the Remind keywords
- use the color palette specified by the user

## Screenshots

### Before

![](https://raw.githubusercontent.com/rkelly/kate-remind/master/before.png "Before syntax coloring")

### After

![](https://raw.githubusercontent.com/rkelly/kate-remind/master/after.png "After syntax coloring")

## Installation

Installation can be as simple as dropping the `kate-remind.xml` file into your Kate `syntax` directory. If your system does not have a `syntax` directory, it may need to be created. The following commands show an example of creating this directory, and copying the file from this repository, directly to where it's needed on your system.

### katepart5/Linux

```bash
mkdir -p ~/.local/share/katepart5/syntax
wget https://gitlab.com/lambdaphile/kate-remind/raw/master/kate-remind.xml \
    -O ~/.local/share/katepart5/syntax/kate-remind.xml
```

### Other Kate Versions/Linux Distros

Other versions of Kate, or other Linux distributions may require you to save the [syntax.xml file](https://gitlab.com/lambdaphile/kate-remind/raw/master/kate-remind.xml) instead to one of the following locations:

#### Linux

- `~/.kde/share/apps/katepart/syntax`
- `/usr/share/kde4/apps/katepart/syntax`

#### Windows

- `%USERPROFILE%\AppData\Local\katepart5\syntax`

After installing the file, *Kate must be restarted* before it will read it.

Syntax highlighting will automatically start when opening a `*.rem` or `*.remind` file. It can also be set manually (eg. if you use a different file suffix) in the bottom right corner of the Kate window. The Remind syntax can be found in the Scripts folder.

## Status

This definition is usable as-is, but is by no means complete. Contributions are welcome.
