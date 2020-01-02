---
layout: artilcle
title:  "vim dracula theme setting"
date:   2019-01-05 22:37:36
categories: book
comment: false
tags: vim
---

## 사용법

* https://draculatheme.com/vim/

dracula.vim을 받아서 ~/.vim/colors에 넣으면 동작한다.

변수 type에만 배경색이 다른 문제가 생김 - .vimrc에 추가하기

~~~vim
let g:dracula_italic = 0
colorscheme dracula
highlight Normal ctermbg=None
~~~

## 출처
* https://github.com/dracula/vim/issues/65
