---
layout: post
title: pathoge-manage your runtimepath with vim
category: linux
tag: [vi, vim]
---
pathogen is build for manage your 'runtimepath' with ease.  In practical terms, pathogen.vim makes it super easy to install plugins and runtime files in their own private directories.

offical homepage is [vim-pathogen](http://www.vim.org/scripts/script.php?script_id=2332).
you can get it from github [github-pathogen](https://github.com/tpope/vim-pathogen).
it's qute simple to install:
~~~~~~~~~~~~~~~~~~~~~~ {.bash}
mkdir -p ~/.vim/autoload ~/.vim/bundle; \
curl -Sso ~/.vim/autoload/pathogen.vim \
    https://raw.github.com/tpope/vim-pathogen/master/autoload/pathogen.vim
~~~~~~~~~~~~~~~~~~~~~~
add this to your vimrc
~~~~~~~~~~~~~~~~~~~~~~~~~ {.bash}
execute pathogen#infect()
syntax on
filetype plugin indent on
~~~~~~~~~~~~~~~~~~~~~~
enjoy!!
