# My vim settings

It's my vim settings on Linux/OSX

## Dependence

* vim
* git

***

## Install

This step will overwrite your .vimrc .gvimrc file and .vim folder, be sure **backup your vim settings** first !!!

    git clone git://github.com/huobazi/vimrc.git
    cd vimrc 
    chmod +x ./install && ./install

# QA
when you update all ,if you counter Ultsnips need  python > 2.7.you have to restore you vim .
first check your vim  
* vim --version |grep python 
if show -python .which say you need reconfigure your vim.then check you python version(python --version)
* 1.git clone https://github.com/vim/vim.git
* 2.cd vim;cd src;
* 3.make distclean  # if you build Vim before
* 4. ./configure --prefix=/usr/local/bin --with-features=huge --enable-perlinterp=yes --enable-rubyinterp=yes --enable-pythoninterp=yes
Done.
