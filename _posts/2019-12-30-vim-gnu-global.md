---
title:  "vim과 GNU global 연동"
date:   2019-12-30 22:32:54
tags: vim
---

Table Of Content
* content
{:toc}

## GNU Global이란?

vim + cscope조합을 꽤 오랫동안 쓰다가, 바꿔봤다.

gtags.vim이 소스 검색 결과를 좀더 잘 보여준다.

- 변수, 함수의 선언으로 이동
- 구현으로 이동
- 사용한 곳으로 이동
- 파일이름으로 이동

## mkcscope.sh와 비슷하게 script를 만들기

~~~bash
#!/bin/bash
find . -name '*.cpp' -o -name '*.h' > gtags.files
gtags --accept-dotfiles -c -f gtags.files
~~~
mktags.sh로 만들고 실행권한을 준다.
source의 최상위 dir에서 한번 호출해주면 된다.

## Incremental 업데이트 하기

한번 tag database를 만든 다음에는 변경된 소스만 대상으로 db를 업데이트 해준다.

파일이 변경되면, update하게 하면 어떨까?

~~~bash
$ global -vu
~~~

## global 예제

~~~bash
$ global func1                 # definition
$ global -r func2              # reference
$ global 'func[1-3]'           # regular expression
$ global -x func2              # show detail
$ global -xg '#ifdef NDEBUG'   # specific pattern 
$ global -c kmem<TAB><TAB>     # complete command
$ vi `global func1`            # edit files having specified tags.
~~~

## 6.6 최신 버전 설치하기

https://ftp.gnu.org/pub/gnu/global/ 코드 다운로드
~~~bash
$ tar -xvzf global-6.6.tar.gz
$ cd global-6.6
$ ./configure
$ make
$ make install
$ global --version
global (GNU GLOBAL) 6.6
~~~

## References
- [GNU Global Manual](https://www.gnu.org/software/global/manual/global.html)
- [gtags.vim](https://github.com/vim-scripts/gtags.vim)
- [keymap 예제](https://slowstarter80.github.io/vim/2017/07/21/vim_settings.html)
- [script형태로 쓰기](https://vi.stackexchange.com/questions/4835/gnu-global-and-vim)
