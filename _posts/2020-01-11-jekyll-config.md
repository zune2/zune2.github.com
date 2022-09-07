---
title:  "jekyll config 지정하기"
date:   2020-01-11 12:32:54
tags: vim
---


## disqus 지정하기

### _config.yml에 shortname 추가
~~~
disqus_shortname: "XXXXXXX" 
~~~

### disqus comment 없애기

post를 작성할 때, 상단 config에 nocomments를 지정함

~~~yaml
nocomments: true
~~~

보이는 것은 default지정

## tag 기능 추가

Tag를 Category아래 추가한다.

~~~yaml
header:
  links:             # Links on the header. Link to in-site page with a slash as prefix
    About: /about/
    Category: /category/
    Tag: /tag/
~~~

tag.html 파일을 만들고, Jekyll template engine 문법에 맞춰서 코딩


## 수학식 출력 (Mathjax)

$$ x = y^2 $$