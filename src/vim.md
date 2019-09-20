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
* External tools integration
  * [vim-gitgutter](https://github.com/airblade/vim-gitgutter)
    * signs of changed lines
    * jumping between the hunks: `[c`, `]c`
    * preview/stage/undo hunk: `<leader>hp`, `<leader>hs`,`<leader>hu`
    * hunk text object: `ic`, `ac`
    * folding unchanged text: `:GitGutterFold`
* Other
  * [Goyo](https://github.com/junegunn/goyo.vim)
    
