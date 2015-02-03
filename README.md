Based on the stackoverflow snippet by Mykola Golubyev:
http://stackoverflow.com/questions/741814/move-entire-line-up-and-down-in-vim/741819#741819

Example keymapping you can put in your ~/.vimrc (although the plugin is already configured to map this may not want to force that on people though)

```
nnoremap <silent> <c-s-up> :call <SID>swap_up()<CR>
nnoremap <silent> <c-s-down> :call <SID>swap_down()<CR>
vnoremap <silent> <c-s-up> <esc>:call <SID>swap_visual_up()<CR>
vnoremap <silent> <c-s-down> <esc>:call <SID>swap_visual_down()<CR>
```
