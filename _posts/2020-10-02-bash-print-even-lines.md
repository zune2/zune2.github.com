---
title:  "text file의 홀수 행만 출력하기"
date:   2020-10-02 12:32:54
tags: bash
---

## 홀수행만 출력하기

~~~bash
sed -n 1~2p ~/test2.txt
~~~


## 짝수행만 출력하기

~~~bash
sed -n 2~2p ~/test2.txt
~~~



## Reference
[Link](https://unix.stackexchange.com/questions/26723/print-odd-numbered-lines-print-even-numbered-lines)