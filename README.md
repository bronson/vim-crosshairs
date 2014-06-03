## Vim Crosshairs

This plugin displays a crosshair over the cursor, similar to having
the cursorline or cursorcolumn settings enabled.  The trick is, the
crosshairs are only visible in the active window.  This can be handy
when you're lost in a sea of splits, vsplits, and quickfix windows.


### TODO

- Update the docfile!!


### Installation

Using Pathogen:

   git clone https://github.com/bronson/vim-crosshairs ~/.vim/bundle/vim-crosshairs

By default the crosshairs won't be shown.  You must enable line, column,
or both in your vimrc like this:

    :set cursorline    " enable the horizontal line
    :set cursorcolumn  " enable the vertical line


### Use

To disable the crosshairs for the current window:

    :setlocal nocursorline
    :setlocal nocursorcolumn

Or globally:

    :set nocursorline
    :set nocursorcolumn

And to force the crosshairs to always be visible in a particular window,
set a window-local variable

    :let w:persistent_cursorline = 1


### Origin

Forked from https://github.com/vim-scripts/CursorLineCurrentWindow
which is a copy of http://www.vim.org/scripts/script.php?script_id=4178


### License

Same as the upstream plugin: Vim License, Charityware.
