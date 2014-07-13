Title: [retext] Retext 的安裝與設定
Date: 2014-06-16 00:00
Modified: 2014-06-16 00:00
Slug: [retext]_retext_install_and_configure
Category: retext
Author: Chris Yang

Retext 是一個好用的 Markdown 編輯器

支援同步瀏覽

內建  apt-get  所安裝的版本是2.0

如果要安裝  4.0的話

安裝方式如下

    sudo add-apt-repository ppa:mitya57
    sudo apt-get update
    sudo apt-get install retext
    
如果是  ubuntu 12.04  安裝的話會有  dependency

可以用  <code>aptitude</code>  來解決缺少python3-pyqt4的問題

aptitude  會提供幾種策略解決，在筆者的環境是先按 N  再按  Y  

使用第二種策略才解決成功

參考來源：<a href="http://www.webupd8.org/2012/03/retext-30-released-text-editor-for.html" target="_blank">ReText 3.0 Released (Text Editor For Markdown And reStructuredText)</a>

安裝好之後 Retext  本身對於  markdown  的  css 跟 github 上差很多

所以要做以下設定

    vim ~/.config/ReText Project/ReText.conf

    [General]
    useReST=false
    defaultExt=md
    useWebkit=true
    styleSheet=/home/自己的家目錄/.config/ReText project/github.css
    
github.css  可以到  <a href="https://gist.github.com/andyferra/2554919" target="_blank">github.css</a>  下載

如此就可以得到支援  github css  格式的  markdownn編輯器

參考來源：<a href="http://whatever1992.blog.163.com/blog/static/21783208820134212303582/" target="_blank">配置Retext</a>


