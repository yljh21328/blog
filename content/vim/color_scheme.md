Title: [vim] 安裝顏色模板 color scheme
Date: 2014-07-01 00:00
Modified: 2014-07-01 00:00
Slug: [vim]_color_scheme
Category: vim
Author: Chris Yang

預設的 vim 顏色很難看

利用 color scheme 可以讓 vim 長的好看一些

可以在 <a href="http://cocopon.me/app/vim-color-gallery/" target="_blank"> Vim Colorscheme Gallery</a> 找一個適合自己的模板

我是用 jellybeans

安裝方式如下

    下載 jellybeans.vim
    mkdir ~/.vim/colors
    mv jellybeans.vim ~/.vim/colors
    
然後設定.vimrc

    vim ~/.vimrc
    
    colorscheme jellybeans
    set t_Co=256
    syntax on


參考來源：
<a href="http://blog.longwin.com.tw/2009/03/choose-vim-color-scheme-2009/" target="_blank">挑選 Vim 顏色(Color Scheme)</a>





