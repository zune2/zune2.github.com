---
layout: post
title:  "cscope와 mkcscope.sh"
date:   2020-01-04 22:32:54
tags: vim
---

vim + cscope조합을 오래 썼다.

적당히 유용하고, indexing된 파일을 분리해서 만들어, 연결해 쓸 수 있다는 장점이 있다.

cscope 커맨드라인도구를 따로 쓸 수 있음. (코드 분석 목적)



## mkcscope.sh로 만들기
~~~bash
#!/bin/sh
rm -rf cscope.files cscope.files
find `pwd` \( -name '*.c' -o -name '*.cpp' -o -name '*.cc' -o -name '*.h' -o -name '*.y' -o -name '*.s' -o -name '*.S' \) -print > cscope.files
cscope -b -i cscope.files
~~~
mkcscope.sh로 만들고 실행권한을 준다.
source의 최상위 dir에서 한번 호출해주면 된다.

vim에서 reset해서 업데이트된 cscope DB를 들고올 수 있다.
~~~
:cs reset
~~~

## References
- [ctags and cscope 사용법](https://wonjaek.tistory.com/65)
