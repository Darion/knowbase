# Vim

## Links

* [Vim github repo](https://github.com/vim/vim)
* [Neovim](https://neovim.io/)
* [Vimways](https://vimways.org/) -- Vim-themed advent calendar
* Books
  * Steve Losh -- [Learn Vimscript the Hard Way](http://learnvimscriptthehardway.stevelosh.com/)
  * Drew Nell -- Practical Vim: Edit Text at the Speed of Thought
  * Drew Nell -- Modern Vim: Craft Your Development Environment with Vim 8 and Neovim

## Plugins

* Basic
  * [vim-surround](https://github.com/tpope/vim-surround)
    * `cs` -- change surround
    * `ds` -- delete surround
    * `ys` -- create surround
    * `.` works if `repeat.vim` installed
  * [vim-repeat](https://github.com/tpope/vim-repeat)
    * `.` command support for some plugins
  * [vim-sneak](https://github.com/justinmk/vim-sneak)
    * `s{char}{char}` -- search place with this two characters, `;` to go to next match
    * `S` -- search backwards
* Search
  * [CtrlSF](https://github.com/dyng/ctrlsf.vim)
    * You can edit search results in-place
    * `CtrlSF needle`
    * `CtrlSFOpen`/`CtrlSFToggle` -- open/toggle window with last search results
    * Search results window keybindings:
      * `Enter`/`o` -- open file and close search window
      * `O` -- open file and leave search window opened
      * `P` -- preview
      * `u` -- undo changes
      * `:w` -- save all changes
      * `q` -- close search window
      * `M` -- toggle regular search results window with quickfix window
      * `<C-J>`/`<C-K>` - next/previous search match
    * Another commands you may want to bind
      * `<Plug>CtrlSFVwordExec` -- find visually selected word
      * `<Plug>CtrlSFCCwordPath` -- find word under the cursor, with word boundaries
* UI
  * [terminus](https://github.com/wincent/terminus)
  * [vim-airline](https://github.com/vim-airline/vim-airline)
  * [vim-startify](https://github.com/mhinz/vim-startify)
* Code
  * [vim-commentary](https://github.com/tpope/vim-commentary)
    * `gc` -- (toggle)comment target of a motion
    * `gcc` -- (toggle)comment strings
    * `gcgc` -- uncomment a set of adjacent commented lines
    * Supports arbitrary filetypes, you just need to set `commentstring` option
    * TODO: 
      * `:7,17Commentary`
      * `:g/TODO/Commentary`
  * [vim-pythonsense](https://github.com/jeetsukumaran/vim-pythonsense)
    * `]]` -- beginning of next class
    * `]m` -- beginning of next function/method
* External tools integration
  * [vim-gitgutter](https://github.com/airblade/vim-gitgutter)
    * signs of changed lines
    * jumping between the hunks: `[c`, `]c`
    * preview/stage/undo hunk: `<leader>hp`, `<leader>hs`,`<leader>hu`
    * hunk text object: `ic`, `ac`
    * folding unchanged text: `:GitGutterFold`
* Other
  * [Goyo](https://github.com/junegunn/goyo.vim)
* Plugins to consider    
  * [vim-multiple-cursors](https://github.com/terryma/vim-multiple-cursors)
