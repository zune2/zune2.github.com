---
layout: page
title:  "elisp - hello world 예제"
date:   2020-01-02 22:32:54
categories: emacs elisp
comments: true
---

## elisp로 hello world 출력하기

M-x ielm으로 모드를 진입하고, 함수를 만들어 본다.

~~~lisp
*** Welcome to IELM ***  Type (describe-mode) for help.
ELISP> (defun say-hello ()
"hello")
say-hello
ELISP> (say-hello)
"hello"
~~~

## list를 만들기

~~~
ELISP> '(rose violet daisy buttercup) 
(rose violet daisy buttercup) 
ELISP>
~~~

## emacs에서 2+2 evalute하기

블럭을 지정한 후, C-x C-e하면 evalute된다.
~~~
(+ 2 2)
~~~

## Reference
- [Practical Emacs Lisp](http://ergoemacs.org/emacs/elisp.html)
- [elisp_basics](http://ergoemacs.org/emacs/elisp_basics.html)
- [Emacs Lisp for Hackers: Hello World](http://joelmccracken.github.io/entries/emacs-lisp-for-hackers-next/)
- [Manual > Lisp-Lists](https://www.gnu.org/software/emacs/manual/html_node/eintr/Lisp-Lists.html#Lisp-Lists)
- [Manual > Run-a-Program](https://www.gnu.org/software/emacs/manual/html_node/eintr/Run-a-Program.html#Run-a-Program)
