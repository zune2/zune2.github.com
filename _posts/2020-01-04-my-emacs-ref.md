---
layout: post
title: "My Emacs Reference Card"
date: 2020-01-04 00:07:54
tags: emacs
---

주로 쓰는 emacs 명령어 정리

## basic command

| CMD	                         | DESC                      |
|--------------------------------|---------------------------|
| C-x C-f                        | 파일 Open                 |
| C-x C-s                        | 파일 Save                 |
| M-x package-list-packages      | package list로 진입하기   |
| C-n                            | 아래로 이동               |
| C-f                            | 오른쪽으로 이동           |
| C-b                            | 왼쪽으로 이동             |
| C-p                            | 위로 이동                 |
| C-d                            | 한 글자 지우기            |
| C-k C-y                        | 한줄 지우고, 붙이기       |
| C-SPC                          | visual block 지정 시작    |
| C-x C-b                        | Buffer List 열기          |
| C-x o                          | 창분할된 옆창 이동        |



## org-mode command

| CMD	                         | DESC                      |
|--------------------------------|---------------------------|
| org-agenda 진입 후 m           | tag를 이용한 검색         |
| F12                            | org-todo-list 진입        |
| C-c C-w                        | refile하기                |




## emacs config mapping

### F11, F12를 org-todo-list, agenda로 매핑하기
~~~elisp
(global-set-key (kbd "<f12>") 'org-todo-list)
(global-set-key (kbd "<f11>") 'org-agenda)
~~~

### refile target이되는 파일 이름 지정하기
~~~elisp
(setq org-refile-targets '(("archive.org" :level . 1)))
~~~

