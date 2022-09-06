---
title: "bash 코딩할 때 도움되는 것들 모아두기"
toc: true
date:   2019-01-05 17:18:44
categories: script
comment: false
tags: bash
---

Table Of Content
* content
{:toc}

## md 확장자인 파일을 찾아서 string 바꾸기, (sub dir모두)
~~~bash
$find . -name "*.md" -exec sed -i -e 's/AAA/BBB/g' {} \;
~~~

- [link](https://stackoverflow.com/questions/1583219/how-to-do-a-recursive-find-replace-of-a-string-with-awk-or-sed)

## scp로 파일 복사하기

~~~bash
sshpass -p암호 scp -o StrictHostKeyChecking=no hello.txt id@111.222.333.444:/home/id/hello.txt
~~~

- expect + scp로도 가능할 것.
- [link](https://zetawiki.com/wiki/%EB%A6%AC%EB%88%85%EC%8A%A4_scp_%EC%9E%90%EB%8F%99%ED%99%94)

## sftp로 최신 파일 가져오기

- wild card 규칙을 적용할 수 있을까?
~~~bash
fileName=$(echo "ls -1rt" | sftp -oIdentityFile=<pathToKeyFile> username@sftpServer:/remoteDir | tail -1) 
~~~

- [link](https://stackoverflow.com/questions/35545774/get-latest-file-from-sftp-to-local-machine)


## References
### Heredoc 관련
1. [how-can-i-write-a-heredoc-to-a-file-in-bash-script](https://stackoverflow.com/questions/2953081/how-can-i-write-a-heredoc-to-a-file-in-bash-script) : heredoc 이용하기
2. [How can I write a heredoc to a file in Bash script?](https://stackoverflow.com/questions/2953081/how-can-i-write-a-heredoc-to-a-file-in-bash-script) : heredoc으로 file생성하기

### GetOpt 관련
2. [An example of how to use getopts in bash](https://stackoverflow.com/questions/16483119/an-example-of-how-to-use-getopts-in-bash) : getopt로 argument처리

### pushd/popd
1. [Can I call pushd/popd and prevent it printing the stack?](https://serverfault.com/questions/108154/can-i-call-pushd-popd-and-prevent-it-printing-the-stack)
