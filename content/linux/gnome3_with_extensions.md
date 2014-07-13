Title: [linux] Gnome3 與 Extensions
Date: 2014-06-08 00:00
Modified: 2014-06-08 00:00
Slug: [linux]_gnome3_with_extensions
Category: linux
Author: Chris Yang

Ubuntu 12.04  預設的桌面是 Unity

而習慣 Gnome 2  或想嘗試  Gnome 3  的朋友可以用下列指令安裝

    sudo add-apt-repository ppa:gnome3-team/gnome3
    sudo apt-get update
    sudo apt-get install gnome-shell
    
參考來源：<a href="http://www.filiwiese.com/installing-gnome-on-ubuntu-12-04-precise-pangolin/" target="_blank">Installing Gnome 3 on Ubuntu 12.04 (Precise Pangolin)</a>
 
安裝完之後就有 Gnome  與 Gnome classic  可以選了

而 Gnome 3  有一個很好玩的東西

叫做 Gnome Shell Extensions

所有的 Extensions  都是用  javascript  寫的

而安裝 extension  的方式非常簡單

只要到  <a href="https://extensions.gnome.org/" target="_blank">GNOME Shell Extensions</a>  點選安裝即可

下面列一下所有我安裝的extensions

- Advanced Settings in UserMenu

這個可以開啟Gnome3的進階設定
 
但是要先安裝 gnome-tweak-tool

<code>sudo apt-get install gnome-tweak-tool</code>

- Advanced Volume Mixer

- Alternative Status Menu

- Axe Menu

- Coverflow Alt-Tab

- Dash to Dock

- Extension List

- Hot-Corn-Dog

安裝這個原本左上角的  Activity Hot Corner  會跑到左下角

- Impatience

加速 gnome-shell animation

- Places Status Indicator

- Removable Drive Menu

- Remove Accessibility

- Remove Activities Button

- Show Desktop Button

- Weather

- Window options

參考來源：<a href="http://maxubuntu.blogspot.tw/2012/09/debian-gnome3.html" target="_blank">Debian Gnome3桌面筆記</a>
