### Github놀이터
***
- vim, emacs conf 올려놓기
- tmux conf 올려놓기
- Emacs org-mode사용한 것 기록하기
- markdown 써보기 
  - http://scriptogr.am/myevan/post/markdown-syntax-guide-for-scriptogram
  - Table of contents를 만들어주는 tool ?
  - 한 페이지에서 다른 페이지로 link하기
- org2blog와 wordpress연동하기. -> Github에도 가능할까?
- jekyll로 만들어보기
- Ruby Version Manager (https://rvm.io/rvm/basics)

### 2015.2.7 jekyll test하기
***
설치가 잘 안됨. Ruby는 처음 써본다. 

### 2015.2.7 Markdown으로 code listing을 나타내기
***
그럭저럭 간결하게 나온다. 
```
echo "hello world"
```

* DILLINGER에서 GITHUB로 연동은 왜 안되는걸까? 혹시 유료? 
* 버튼을 눌러도 저장이 안되는 것처럼 보임.

### 2015.2.7 Coding할 땐 Tmux+Vim, Management는 Emacs에서 org-mode
***
org모드로 일정관리와 노트정리를 하고, 프로그래밍은 Tmux에서 vim으로 하고있다. 0~9까지 10개의 가상 터미널이 하나의 terminal에서 동작하므로 모니터 하나만 봐도 다양한 작업을 할 수 있어서 좋다.

### 2015.2.7 Emacs기반 markdown 에디터
***
- https://www.youtube.com/watch?v=qnoMo0ynyZo
- websocket과 web framework를 엮어서 Preview가 지원되는 Emacs기반 markdown 에디터

### 2015.2.7 http://dillinger.io/ Web기반 markdown에디터
***
Web browser만 있으면, 미리보기가 되면서 문서를 쓸 수 있다.

### 2015.2.6 Emacs에서 IRC를 해보다.
***
재미난 시도. 이맥스의 끝은 어디인가?

### 2015.2.6 Emacs deft.el
***
org mode와 asciidoc등 구분없이 지원하는 note-taking시스템이다. org-capture가 더 익숙하지만, 이건 page별 검색도 지원하는 위키같은 느낌이 든다.

### 2015.2.6 Github에 web page만들다.
***
Github에서 web site를 만들어보았다. markdown으로 HTML작성없이도 페이지를 만들 수 있다.
http://dillinger.io/에서 page preview를 보면서 작성해서 옮기면 된다.

markdown형태로 한 page짜리 page를 만들어도 개인 blog로 충분하지 않을까 싶다.

### 2015.2.5 org mode로 calendar와 연동해서 보다.
***
Emacs org mode에서 calendar를 org mode와 연동하는 것이 가능하다.  더 예쁘게 볼 수 있지만, 그다지 유용하지는 않았다. '아~ 이런 것도 되는구나' 정도랄까?

### 2015.2.4 org-agenda-todo를 키맵하다.
***
Emacs org mode에서 org-agenda-todo를 F12키로 map하고나니, 일정을 보는게 한결 편해졌다. 자주 체크하는 것이 좋다.

### 2015.2.3 Emacs와 Cscope를 연동하다.
***
GNU Global로 해볼까 하다가 그냥 익숙한 Cscope를 Emacs에 연동해봄. xcscope.el 패키지를 설치하면, 쉽게 할수 있다. 하지만 vim보다 아직 키맵이 익숙하지 않고 불편한 상태.

### 2015.1.25 VIM vundle와 pathogon
***
전통적인 vim의 dir과 다르게 구성. git에서 받아서 패키지를 구성하도록 했다. 파일이 서로 섞이지 않도록 한 것이 주요해보인다.

### 2015.1.21 org-mode ARCHIVE tag이용하기
***
ARCHIVE태그를 주면, html 생성할 때, 추가되지 않는다. '가려주는 것'도 유용한 기능이다. 백업을 따로 하는 것은 귀찮은 일이니까.

### 2015.1.19 org-mode에서 snippets 사용하기
***
code listing을 적을 때 편리한 기능이다. YASnippets도 같이 확인해볼 필요가 있음.

### 2015.1.13 Emacs에서 batch mode로 org-mode를 HTML로 export하기
***
Makefile에 추가완료함. 근데 왜 HTML export명령이 예전 것이 될까?

### 2015.1.11 Emacs list in 15min 따라해봄
***
이맥스 Lisp을 요리책처럼 따라해볼 수 있는 구성.
defun, mapcar, car, prog등을 배울 수 있다.

### 2015.1.5 info 뷰어로 Emacs 이용하기
***
docbook으로 info만드는 방법이 있다. bash commands 설명이 info가 man보다 설명이 더 풍부한 것 같다.

    Ctrl-h i

### 2014.12.22 vim script Hello World 해보기
***
vim script와 Emacs lisp와 어떤 차이가 있는지 감으로 파악하기.
