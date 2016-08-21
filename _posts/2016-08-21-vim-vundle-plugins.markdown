---
layout: post
title:  "Vim Vundle로 플러그인 설치하기"
date:   2016-08-21 12:14:00
categories: Hobby
comments: true
---

기존에 한곳의 dir에서 나눠서 저장하던 구조를 플러그인 별로 하나의 dir을 두고, git에서 가져와서 쉽게 설치할 수 있다.

	" :PluginInstall 명령으로 설치를 함

	" Vim bundle  ------------------------
	set rtp+=~/.vim/bundle/Vundle.vim
	call vundle#rc()

	Plugin 'tpope/vim-fugitive'
	Plugin 'scrooloose/nerdtree.git'
	Plugin 'vim-scripts/c.vim'
	filetype plugin indent on " required

기존에 vim.org의 script에서 받아서 설치하는 것보다 편리하다.
c.vim으로 plugin을 받아서 설치함. git은 어느 경로에서 가져오는지 알아볼 것.
github가 기본인 것으로 보인다.
