set ai
set hlsearch
set history=100
set et
set ts=4
set sw=4
set smarttab
set ruler
set backspace=2
filetype on
filetype plugin on
filetype plugin indent on
syntax on
set ls=2
set background=dark
set statusline=%.40F[%{strlen(&fenc)?&fenc:'none'},%{&ff}]%h%m%r%y%=%c,%l/%L\ %P
function! ResCur()
  if line("'\"") <= line("$")
    normal! g`"
    return 1
  endif
endfunction

nnoremap <F2> :set invpaste paste?<CR>
set pastetoggle=<F2>
set showmode

augroup resCur
  autocmd!
  autocmd BufWinEnter * call ResCur()
augroup END
