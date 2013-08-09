---
layout: post
title: complete java code with vim
category: linux
tag: [vi, vim]
---
Javacomplete is javacomplete, an omni-completion script of JAVA language for vim 7.

offical homepage is [vim-javacomplete](http://www.vim.org/scripts/script.php?script_id=1785).

~~~~~~~~~ {.bash}
unzip javacomplete0.77.1.2.zip -d ~/.vim
~~~~~~~~~~~~~~~~~~~~~~

add this to your vimrc($HOME/.vimrc or /etc/vim/vimrc)

~~~~~~~~~ {.bash}
setlocal omnifunc=javacomplete#Complete
setlocal completefunc=javacomplete#CompleteParamsInfo
autocmd Filetype java,javascript,jsp inoremap <buffer>. .<C-X><C-O><C-P><Down>
~~~~~~~~~~~~~~~~~~~~~~

when first used,Reflection.java will be automatcally compiled and placed to $HOME.
