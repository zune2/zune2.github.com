---
layout: post
title:  "my-vim-tips"
date:   2019-01-05 22:47:15
categories: script
comments: false
tags: vim
---

### trailing white spaces 지우기 (in place)

```
:%s/\s\+$//e
```

### 여러 파일 열기 (in place)  / buffer 이동

```
: args a.txt b.txt        :bn 
```

### F10으로 파일 내용 클립보드 복사 (.vimrc)

```
map <F10> <ESC>:!xsel --clipboard --input < % <CR><CR>
```

