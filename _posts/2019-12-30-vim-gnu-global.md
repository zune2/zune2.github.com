---
title:  "vim과 GNU global 연동"
date:   2019-12-30 22:32:54
categories: vim

---

## GNU Global이란?

vim + cscope조합을 꽤 오랫동안 쓰다가, 바꿔봤다.

gtags.vim이 소스 검색 결과를 좀더 잘 보여준다.

- 변수, 함수의 선언으로 이동
- 구현으로 이동
- 사용한 곳으로 이동
- 파일이름으로 이동

## mkcscope.sh와 비슷하게 script를 만들기

~~~bash
find . -name '*.cpp' -o -name '*.h' > gtags.files
gtags --accept-dotfiles -c -f gtags.files
~~~
mktags.sh로 만들고 실행권한을 준다.
source의 최상위 dir에서 한번 호출해주면 된다.

## References
- [gtags.vim](https://github.com/vim-scripts/gtags.vim)
- [keymap 예제](https://slowstarter80.github.io/vim/2017/07/21/vim_settings.html)
- [script형태로 쓰기](https://vi.stackexchange.com/questions/4835/gnu-global-and-vim)
