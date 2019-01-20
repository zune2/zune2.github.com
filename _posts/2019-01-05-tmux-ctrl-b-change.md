---
layout: post
title:  "tmux ctrl-b키를 ctrl-a키로 변경하기"
date:   2019-01-05 22:21:47
categories: script
comments: false
tags: tmux
---

.tmux.conf에 다음을 추가한다.

~~~
unbind C-b                                                                                                                                                           
set -g prefix C-a                                                                                                                                                    
bind C-a send-prefix
~~~

