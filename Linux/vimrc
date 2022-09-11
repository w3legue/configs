set nocompatible              " be iMproved, required
filetype off                  " required

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()
Plugin 'VundleVim/Vundle.vim'

" Git pluggins
Plugin 'tpope/vim-fugitive'
" Status and tabline
Plugin 'vim-airline/vim-airline'

" Nerd Tree
Plugin 'scrooloose/nerdtree'

call vundle#end()

" Nerd Tree maps
let NERDTreeIgnore = ['__pycache__', '\.pyc$', '\.o$', '\.so$', '\.a$', '\.swp', '*\.swp', '\.swo', '\.swn', '\.swh', '\.swm', '\.swl', '\.swk', '\.sw*$', '[a-zA-Z]*egg[a-zA-Z]*', '.DS_Store', '\idea', '\.iml']
let NERDTreeShowHidden=1
let g:NERDTreeWinPos="left"
let g:NERDTreeDirArrows=0
let g:NERDTreeNodeDelimiter = "\u00a0"  "Gets rid of ^G at the start of every line
:nmap <c-e> :NERDTreeToggle<CR>

" Tab Movement
set tabstop=2
set shiftwidth=2
set softtabstop=2
set expandtab
set smartindent
set incsearch
set smartcase
set nu

" set relativenumber
set backspace=2
set ruler
set hlsearch
set wildchar=<Tab> wildmode=full
set wildmenu
syntax on
set showcmd
autocmd FileType python set tabstop=2|set shiftwidth=2|set expandtab|set backspace=2|set softtabstop=2
autocmd BufWritePre * :%s/\s\+$//e

"Clear search highlights. The only way I will use highlite search (hlsearch)
map <leader><space> :let @/=''<cr>

" Run the json formating tool
nmap <leader>jf :%!python -m json.tool indent=2<CR>
nmap <leader>jq :%!jq -S .<CR>

" Change splits to right and below as default
set splitright
set splitbelow
" Split navigations
nnoremap <C-J> <C-W><C-J>
nnoremap <C-K> <C-W><C-K>
nnoremap <C-L> <C-W><C-L>
nnoremap <C-H> <C-W><C-H>

" Enable folding
set foldmethod=indent
set foldlevel=99

" Enable folding with the spacebar
nnoremap <space> za
