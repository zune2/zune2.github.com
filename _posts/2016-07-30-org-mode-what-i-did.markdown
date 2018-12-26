---
layout: post
title:  "org-mode 해본 것들"
date:   2016-07-30 11:13:00
categories: Hobby
comments: true
---
<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
**Table of Contents**

- [-](#-)
- [org mode로 calendar와 연동해서 보다.](#org-mode로-calendar와-연동해서-보다)
- [DONE org-agenda-todo를 키맵하다.](#done-org-agenda-todo를-키맵하다)
- [DONE org-mode ARCHIVE tag이용하기](#done-org-mode-archive-tag이용하기)
- [org-mode에서 snippets 사용하기](#org-mode에서-snippets-사용하기)
- [DONE org-mode에 plantuml을 이용해서 UML 다이어그램 그리기](#done-org-mode에-plantuml을-이용해서-uml-다이어그램-그리기)

<!-- markdown-toc end -->


## DONE org-agenda-todo를 전체 화면으로 보기
***
.emacs에서 window를 current로 지정하면 됨
{% highlight lisp %}
(setq org-agenda-window-setup 'current-window)
{% endhighlight %}
[emacs-org-agenda-list-destroy-my-windows-splits](http://stackoverflow.com/questions/10635989/emacs-org-agenda-list-destroy-my-windows-splits)


## org mode로 calendar와 연동해서 보다.
***
- 2015.2.5
- Emacs org mode에서 calendar를 org mode와 연동하는 것이 가능하다.  더 예쁘게 볼 수 있지만, 그다지 유용하지는 않았다. '아~ 이런 것도 되는구나' 정도랄까?

## DONE org-agenda-todo를 키맵하다.
***
- 2015.2.4
- Emacs org mode에서 org-agenda-todo를 F12키로 map하고나니, 일정을 보는게 한결 편해졌다. 자주 체크하는 것이 좋다.

## DONE org-mode ARCHIVE tag이용하기
***
- 2015.1.21
- ARCHIVE태그를 주면, html 생성할 때, 추가되지 않는다. '가려주는 것'도 유용한 기능이다. 백업을 따로 하는 것은 귀찮은 일이니까.

~~~~~~
C-w C-w : refiling
~~~~~~

## org-mode에서 snippets 사용하기
***
- 2015.1.19
- code listing을 적을 때 편리한 기능이다. YASnippets도 같이 확인해볼 필요가 있음.

## DONE org-mode에 plantuml을 이용해서 UML 다이어그램 그리기
***
- 2015.2.11
- 그림을 그리지 않고, textual description으로 diagram을 생성할 수 있어서, 유용했다.


