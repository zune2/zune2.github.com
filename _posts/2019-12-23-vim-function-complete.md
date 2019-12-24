---
layout: post
title:  "clang_complete 이용하기"
date:   2019-12-23 22:32:54
categories: vim
comments: true
---
# content
{:toc}

## 사용법
  - 함수 이름 + Ctrl-x Ctrl-u 입력

## .vimrc에 플러그인 설치하기

    Plugin 'SirVer/ultisnips'
    Plugin 'Valloric/YouCompleteMe'
    Plugin 'xavierd/clang_complete'
    Plugin 'ervandew/supertab'

## .vimrc에 syntastic, clang_complete 설정하기

    " Syntastic
    set statusline+=%#warningmsg#
    set statusline+=%{SyntasticStatuslineFlag()}
    set statusline+=%*

    "let g:syntastic_always_populate_loc_list = 1
    let g:syntastic_auto_loc_list = 1
    let g:syntastic_check_on_open = 1
    let g:syntastic_check_on_wq = 0

    let g:syntastic_cpp_check_header = 1
    let g:syntastic_cpp_compiler = 'g++'
    let g:syntastic_cpp_compiler_options = "-std=c++11 -Wall -Wextra -Wpedantic"
    let g:syntastic_c_compiler_options = "-std=c11 -Wall -Wextra"

    let g:syntastic_c_check_header = 1
    let g:syntastic_c_clang_check_post_args = ""
    let g:syntastic_clang_check_config_file = "./compile_commands.json"
    "---------------------------------------------------------------
    "colorscheme	morning

    let g:clang_library_path='/usr/lib/llvm-3.8/lib'

    set pumheight=10             " so the complete menu doesn't get too big
    set completeopt-=preview
    set completeopt=menu,longest " menu, menuone, longest and preview

    let g:SuperTabDefaultCompletionType='context'
    let g:clang_complete_auto=0  " I can start the autocompletion myself, thanks..
    let g:clang_snippets=1       " use a snippet engine for placeholders
    let g:clang_snippets_engine='ultisnips'
    let g:clang_auto_select=2  

## References
  - https://github.com/xavierd/clang_complete
  - https://www.vim.org/scripts/script.php?script_id=2715

