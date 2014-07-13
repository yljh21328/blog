Title: [linux] 安裝 lubuntu 13.10
Date: 2014-06-09 00:00
Modified: 2014-06-09 00:00
Slug: [linux]_lubuntu_install
Category: linux
Author: Chris Yang

在這邊我安裝的是 lubuntu 13.10 64bit

- <a href="http://cdimage.ubuntu.com/lubuntu/releases/13.10/release/lubuntu-13.10-desktop-amd64.iso" target="_blank">lubuntu 13.10 64-bit 載點</a>

有幾個需要注意的地方

首先先將 lubuntu 的光碟放進光碟機

然後再開機時選擇用光碟機開機

進去之後請選擇用 <code>中文</code> 的方式安裝

如果你安裝的是英文語系的話，那麼到時候你的中文支援會非常的不完整

但是如果你安裝時是用中文安裝的話，到時候安裝的加目錄可以切換回英文的目錄

在磁碟分割的時候可以選擇一個空的區域(我是切100G)，格式化成 <code>ext4</code>

並掛載給根目錄 <code>/</code> 即可

<code>swap</code>的話就看自己要不要切了，現在的記憶體空間應該都是夠用

<code>記得如果要裝雙系統的話要先裝 windows 再裝 ubuntu，不然開機選單會讀不到</code>

安裝完之後有幾件事情要注意一下

- 將中文目錄改回英文名稱
	
	1.echo $LANG
	
	2.export LANG=en_US
	
	3.xdg-user-dirs-gtk-update
	
	4.將第一步驟得到的 $LANG 給 export 回去
	
	參考來源: <a href="http://freedom-heero.blogspot.tw/2012/11/ubuntu.html" target="_blank">蒼天之劍</a>

- 連接網路

- 更新語言支援 language support

- 更新系統： 
	- 先下 <code>sudo apt-get update</code> 更新軟體源再下 <code>sudo apt-get upgrade</code> 更新套件

- 安裝常用軟體：
	- filezilla <code>sudo apt-get install filezilla</code>
	- aptitude <code>sudo apt-get install aptitude</code>
	- lamp sudo <code>apt-get install lamp-server^</code>
	- phpmyadmin <code><a href="http://www.phpmyadmin.net/home_page/index.php" target="_blank">phpmyadmin 官網</a></code>
	- vim sudo <code>apt-get intsll vim</code>
	- ssh sudo <code>apt-get install openssh-server</code>
	- git sudo <code>apt-get install git</code>

- 更新設定檔
	- .bashrc
	- .vimrc
	- .vim
	- .gitignore
	- .ssh