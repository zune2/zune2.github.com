---
title:  "NEERC input/output file 테스트하기"
date:   2020-03-01 22:32:54
categories: ProblemSolving

---

## script로 NEERC 문제 input/output test하기

NEERC는 문제에 대한 input/output file을 제공한다.
다음처럼 script를 이용하면, 손쉽게 pass/fail을 테스트할 수 있다.

~~~bash
#!/bin/bash

./code < tests/disktree.01 | diff ./tests/disktree.01a -
./code < tests/disktree.02 | diff ./tests/disktree.02a -
./code < tests/disktree.03 | diff ./tests/disktree.03a -
./code < tests/disktree.04 | diff ./tests/disktree.04a -
./code < tests/disktree.05 | diff ./tests/disktree.05a -
./code < tests/disktree.06 | diff ./tests/disktree.06a -
./code < tests/disktree.07 | diff ./tests/disktree.07a -
./code < tests/disktree.08 | diff ./tests/disktree.08a -
./code < tests/disktree.09 | diff ./tests/disktree.09a -
./code < tests/disktree.10 | diff ./tests/disktree.10a -
~~~

## Reference
https://neerc.ifmo.ru/archive/2000.html
