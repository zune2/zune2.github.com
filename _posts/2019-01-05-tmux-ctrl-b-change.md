---
title:  "tmux ctrl-b키를 ctrl-a키로 변경하기"
date:   2019-01-05 22:21:47
categories: script
comment: false
tags: tmux
---

## Ctrl a로 키맵변경
기본으로는 Ctrl b로 지정되어 있다.

.tmux.conf에 다음을 추가한다.

```
unbind C-b                                                                                                                                                           
set -g prefix C-a                                                                                                                                                    
bind C-a send-prefix
```

## Emacs 키맵과 충돌 문제

C-a로 라인의 시작으로 이동하는 명령이 연결되어 있다. tmux에서 이맥스를 켜면, C-a를 tmux가 먼저 인식하게 되는 문제가 있다.

~~~
C-a
<Home>
Move to the beginning of the line (move-beginning-of-line).
C-e
<End>
Move to the end of the line (move-end-of-line). 
~~~

## Reference
- [Emacs - Moving Point](https://www.gnu.org/software/emacs/manual/html_node/emacs/Moving-Point.html)
