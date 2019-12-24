---
layout: post
title:  "clang_complete 이용하기"
date:   2019-12-23 22:32:54
categories: vim
comments: true
---

Table of Content
* content
{:toc}

## libclang 설치

    sudo apt-get install libclang-3.8-dev

## .vimrc에 플러그인 설치하기

    Plugin 'SirVer/ultisnips'
    Plugin 'xavierd/clang_complete'

## .vimrc에 clang_complete 설정하기

    let g:clang_library_path='/usr/lib/llvm-3.8/lib'

    set pumheight=10             " so the complete menu doesn't get too big
    set completeopt-=preview
    set completeopt=menu,longest " menu, menuone, longest and preview

    let g:SuperTabDefaultCompletionType='context'
    let g:clang_complete_auto=0  " I can start the autocompletion myself, thanks..
    let g:clang_snippets=1       " use a snippet engine for placeholders
    let g:clang_snippets_engine='ultisnips'
    let g:clang_auto_select=2  

## 사용법
  - 함수 이름 + Ctrl-x Ctrl-u 입력하면, parameter list가 채워진다.

## References
  - https://stackoverflow.com/questions/11300788/vim-function-hints-for-c
  - https://github.com/xavierd/clang_complete
  - https://www.vim.org/scripts/script.php?script_id=2715

