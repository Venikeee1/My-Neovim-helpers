# My-Neovim-helpers
Currently I am using [vim-plug](https://github.com/junegunn/vim-plug) for installing NeoVim plugin

## Common allias

`<Leader>` - default key is back slash `\`

## Vim tabs
`:tabedit FILENAME` - open new tab

`tabe` - open new file

`<C-W>c` - close tab

`:tabo` - close all others tabs

`gt` and `gT` - switch between tans

### My alliases
`<leader>tn` - new tab

`<leader>t<leader>` - next tab

`<leader>to` - leave only one tab

`<leader>tc` - close tab

`<leader>tm #` - move tab

## Telescope
Tool for search in files

```
nnoremap <leader>ff <cmd>Telescope find_files<cr> --- search by file name
nnoremap <leader>fg <cmd>Telescope live_grep<cr> --- search throught files
nnoremap <leader>fb <cmd>Telescope buffers<cr>
nnoremap <leader>fh <cmd>Telescope help_tags<cr>
```


## NerdTree [link](https://github.com/preservim/nerdtree#frequently-asked-questions)
`<C-n>` - open

`<C-t>` - toggle

`<C-f>` - find

`<leader>n` - focus

## NerdComments. [Doc](https://www.vim.org/scripts/script.php?script_id=1218)
`<leader>cc` - Comment out the current line or text selected in visual mode

`<leader>cn` - Same as <leader>cc but forces nesting.

`<leader>c<space>` - Toggles the comment state of the selected line(s). If the topmost selected line is commented, all selected lines are uncommented and vice versa.

`<leader>cm` - Comments the given lines using only one set of multipart delimiters

`<leader>ci` - Toggles the comment state of the selected line(s) individually.

`<leader>cs` - Comments out the selected lines ``sexily''

`<leader>cy` - Same as <leader>cc except that the commented line(s) are yanked first.
  
`<leader>c$` - Comments the current line from the cursor to the end of line.
  
`<leader>cA` - Adds comment delimiters to the end of line and goes into insert mode between them.

`<leader>cu` - Uncomments the selected line(s).

