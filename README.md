# Vim It Up 🔥
### A collection of scripts, plugins, and clever hacks so that you can exit vim in STYLE! 🚀

(Not that you would want to, ever... MUAHAHAHA)

![Vim It Up](vim.png)

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](./CONTRIBUTING.md)

Some of the settings here may reference a 'leader' key, use:
```vim
let mapleader="{Your Key Of Choice}"
```

## Sane-er Defaults

Enables syntax highlighting, why wouldn't you?
```vim
syntax on
```

Shows you line numbers, it's great:
```vim
set number
```

Copy and paste from the **system** clipboard, and avoid indentation issues:
```vim
noremap <leader>y "+y
noremap <leader>p "+p
```

Makes the backspace key behave like you'd expect, and go through EVERYTHING:
```vim
set backspace=indent,eol,start
```

Makes 1 tab = 4 spaces:
```vim
set shiftwidth=4
set tabstop=4
```

## Avoiding RSI

If you use command mode a lot, swapping the colon and semi-colon keys means 1 less keypress:
```vim
nnoremap ; :
nnoremap : ;
```
## Nicer Navigation
Allows the cursor to move up and down naturally by display, lines instead of file lines:
```vim
nnoremap j gj
nnoremap k gk
```

Make yanking with capital Y behave like the other capital letters, and yank until the end of the line:
```vim
nnoremap Y y$
```

## File and Buffer Navigation, but better
Press space twice to switch between your last two buffers, use it all the time for superfast switching:
```vim
nnoremap <leader><leader> <c-^>
```

Switch buffers with Left and Right arrow keys:
```vim
nnoremap <left> :bp<cr>
nnoremap <right> :bn<cr>
```

## Super-Cool Plugins

A fuzzy-finder to easily search for files, contents & buffers:

[junegunn/fzf.vim](https://github.com/junegunn/fzf.vim)

Provides mappings to easily delete, change and add parentheses, brackets, quotes, and tags:

[tpope/vim-surround](https://github.com/tpope/vim-surround)

An integrated git experience in vim, that's "so awesome, it should be illegal":

[tpope/vim-fugitive](https://github.com/tpope/vim-fugitive)
