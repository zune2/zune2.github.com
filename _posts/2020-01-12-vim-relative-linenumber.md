---
title:  "vim relative 라인 번호 지정"
date:   2020-01-12 12:32:54
tags: vim
---

## set rnu이란?
vim에서 행 번호를 현재 커서 기준으로 위 아래를 지정할 하는 기능

~~~vim
set number
set nu
set relativenumber
set rnu     " 켜기
set rnu!    " 끄기
~~~

행 번호가 상대기준으로 보인다면 줄 이동을 여러번 key입력하지 않아도 된다.
~~~
7+    " 7줄 아래로 이동
g-    " 7줄 위로 이동
~~~


## Ctrl-L Ctrl-L을 이용해서 모드 변경하기
~~~
" .vimrc에 키맵을 추가함
" Relative number display
nmap <C-L><C-L> :set invrelativenumber<CR>
~~~

## Reference
[Link](https://vi.stackexchange.com/questions/3/how-can-i-show-relative-line-numbers)