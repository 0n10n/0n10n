# 自己的Linux初装环境设置

## Windows下的Putty sessions 文件设置
这些文件默认在Putty安装目录下的`sessions`子目录。自己习惯需要更改的几个项目：
```
......
TerminalType\linux\
......
Font\Consolas\
FontHeight\12\
......
ANSIColour\1\
Xterm256Colour\1\
TrueColour\1\
......
WinTitle\%25%25h%20%25%25u\
```

## Linux 默认环境设置
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

## 更新github ip hosts表

```
0 1 * * * /root/update_hosts.sh >/dev/null 2>&1
```
