## CursorLine

This plugin displays a crosshair over the cursor, similar to having
the cursorline or cursorcolumn settings enabled, but only in the
active window.  It's hidden when you switch away.


### Installation

Using Pathogen:

   git clone https://github.com/bronson/vim-cursorline ~/.vim/bundle/vim-cursorline

By default the crosshairs won't be shown.  Enable line, column,
or both in your vimrc like this:

    :set cursorline
    :set cursorcolumn


### Use

To disable the crosshair for the current window:

    :setlocal nocursorline
    :setlocal nocursorcolumn

Or globally:

    :set nocursorline
    :set nocursorcolumn

And to force it to always be visible in a particular window,
set this window-local variable

    :let w:persistent_cursorline = 1


### Origin

Forked from https://github.com/vim-scripts/CursorLineCurrentWindow
which is a copy of http://www.vim.org/scripts/script.php?script_id=4178


### License

Same as the upstream plugin: Vim License, Charityware.
