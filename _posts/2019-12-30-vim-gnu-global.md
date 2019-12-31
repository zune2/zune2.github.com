---
layout: post
title:  "vim과 GNU global 연동"
date:   2019-12-30 22:32:54
categories: vim
comments: true
---

cscope를 오래 써오다가 최근에 설치한 소스 검색 도구.

- 변수, 함수의 선언으로 이동
- 구현으로 이동
- 사용한 곳으로 이동

쉽게 할 수 있게 해준다.

### mkcscope.sh와 비슷하게 script를 만들기
mktags.sh를 만들어준다.
~~~
find . -name '*.cpp' -o -name '*.h' > gtags.files
gtags --accept-dotfiles -c -f gtags.files
~~~

source의 최상위 dir에서 한번 호출해주면 된다.

### References
- [gtags.vim](https://github.com/vim-scripts/gtags.vim)
- [keymap 예제](https://slowstarter80.github.io/vim/2017/07/21/vim_settings.html)
- [script형태로 쓰기](https://vi.stackexchange.com/questions/4835/gnu-global-and-vim)
