Title: [vim] vundle 套件管理
Date: 2014-07-02 00:00
Modified: 2014-07-02 00:00
Slug: [vim]_vundle_plugin
Category: vim
Author: Chris Yang

vundle 是一個 vim 的套件管理工具

使用<code>git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim</code>

就可以輕鬆的安裝 Vundle 了

然後再在 .vimrc 中設定即可

    set rtp+=~/.vim/bundle/Vundle.vim
    call vundle#begin()
    Plugin 'gmarik/Vundle.vim'
    call vundle#end()  
    
將要安裝的  plugin  放在  vundle#begin()  與  vundle#end()  之中

然後下

    :source %
    :PluginInstall

即可安裝完成

參考來源：

<a href="https://github.com/gmarik/Vundle.vim" target="_blank">Vundle.vim</a>

<a href="http://vimawesome.com/" target="_blank">VimAwesome</a>




