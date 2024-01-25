# 自己的Linux初装环境设置

## Windows下的Putty设置
TerminalType设置为linux：
```
TCPNoDelay\1\
TCPKeepalives\0\
TerminalType\linux\
TerminalSpeed\38400,38400\
```

## 环境设置
```
cp setting.sh /etc/profile.d/

```

## vim 设置
编辑 /etc/vim/vimrc

```
colorscheme slate
syntax on
set compatible
set number
set virtualedit=block
set expandtab
set shiftwidth=2
set softtabstop=2
set tabstop=2
set showmatch
set cursorline
set cursorcolumn
set ignorecase
set smartcase
set hlsearch
set noerrorbells
set laststatus=2
set guioptions+=a
set smartindent
set noswapfile
filetype on
filetype plugin on
filetype plugin indent on
if filereadable("/etc/vim/vimrc.local")
  endif
```
