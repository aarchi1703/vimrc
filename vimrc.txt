" ===========================
" Плагины
" ===========================
call plug#begin('~/.vim/plugged')


Plug 'preservim/nerdtree'

call plug#end()   

" ===========================
" Клавиши
" ===========================
" Сочетание клавиш для переключения NERDTree
nnoremap <C-b> :NERDTreeToggle<CR>

" Сочетание клавиш для копирования в системный буфер обмена
nnoremap <C-y> "+y
vnoremap <C-y> "+y

" Сочетание клавиш для отключения подсветки поиска
nnoremap <Esc> :nohlsearch<CR>


" Прокрутка + центрирование
nnoremap <C-D> <C-D>zz
nnoremap <C-U> <C-U>zz


" ===========================
" Основные настройки
" ===========================
" Кодировка
set encoding=utf-8
set fileencodings=utf-8

set nocompatible
filetype plugin indent on

" ===========================
" Настройки отображения
" ===========================
set relativenumber
set number
set numberwidth=1

highlight LineNr ctermfg=NONE guifg=NONE
highlight CursorLineNr ctermfg=NONE guifg=NONE

syntax on

set scrolloff=5
set background=dark 

" ===========================
" Настройки табуляции
" ===========================
set expandtab
set tabstop=4 
set shiftwidth=4 
set softtabstop=4

set smarttab
set smartindent

" ===========================
" Языковые настройки
" ===========================
set langmap=ФИСВУАПРШОЛДЬТЩЗЙКЫЕГМЦЧНЯ;ABCDEFGHIJKLMNOPQRSTUVWXYZ,фисвуапршолдьтщзйкыегмцчня;abcdefghijklmnopqrstuvwxyz


" ===========================
" Безопасность
" ===========================
set modelines=0

" ===========================
" Производительность
" ===========================
set backspace=indent,eol,start
set nowrap
set ruler
set mouse=a

" ===========================
" Автокоманды
" ===========================
au BufWrite /private/tmp/crontab.* set nowritebackup nobackup
au BufWrite /private/etc/pw.* set nowritebackup nobackup

" ===========================
" Поиск
" ===========================
set hlsearch
set incsearch
set ic
set smartcase

