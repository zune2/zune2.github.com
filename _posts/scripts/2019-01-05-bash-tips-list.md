---
title: "bash 코딩할 때 도움되는 것들 모아두기"
toc: true
date:   2019-01-05 17:18:44
categories: script
comment: false
tags: bash
---

* content
{:toc}

## md 확장자인 파일을 찾아서 string 바꾸기, (sub dir모두)
~~~bash
$find . -name "*.md" -exec sed -i -e 's/AAA/BBB/g' {} \;
~~~

- [link](https://stackoverflow.com/questions/1583219/how-to-do-a-recursive-find-replace-of-a-string-with-awk-or-sed)

## References
### Heredoc 관련
1. [how-can-i-write-a-heredoc-to-a-file-in-bash-script](https://stackoverflow.com/questions/2953081/how-can-i-write-a-heredoc-to-a-file-in-bash-script) : heredoc 이용하기
2. [How can I write a heredoc to a file in Bash script?](https://stackoverflow.com/questions/2953081/how-can-i-write-a-heredoc-to-a-file-in-bash-script) : heredoc으로 file생성하기

### GetOpt 관련
2. [An example of how to use getopts in bash](https://stackoverflow.com/questions/16483119/an-example-of-how-to-use-getopts-in-bash) : getopt로 argument처리

### pushd/popd
1. [Can I call pushd/popd and prevent it printing the stack?](https://serverfault.com/questions/108154/can-i-call-pushd-popd-and-prevent-it-printing-the-stack)
