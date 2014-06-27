Title: [latex] 在 lubuntu 13.10 上安裝 texlive 與 texstudio
Slug: [latex]_latex_install
Category: latex
Author: Chris Yang

tex 是一個專業的排版格式，通常用來寫論文

而 texlive 是一個用來編譯 tex 的套件

texstudio 則是一套用來寫 tex 的編輯器

- <a href="https://www.tug.org/texlive/" target="_blank">texlive 官網</a>

- <a href="http://texstudio.sourceforge.net/" target="_blank">texstudio 官網</a>

上面兩個連結可以下載 texlive 以及 texstudio

要先安裝 texlive 或 texstudio 都可以

### 安裝 texlive

安裝 texlive 只要解壓縮後執行 <code>sudo ./install-tl</code>

然後提示界面輸入 <code>i</code> 後按確認即可安裝

大概要等上 15 ~ 20 分鐘

安裝完之後在 <code>~/.bashrc</code> 的最後面加上 <code>export PATH=/usr/local/texlive/2014/bin/i386-linux:$PATH </code>

PATH 會因為安裝路徑有異，要仔細注意

存檔之後記得下 <code>source ~/.bashrc</code>

### 安裝 texstudio

從官網依照自己的版本下載完之後解壓縮

利用 <code>dpkg -i xxx.deb</code> 安裝即可

如果有相依性的問題，則改用 <code> gdebi xxx.deb</code> 來安裝

gdebi 可以用來解相依性的問題

如果打開 texstudio 上邊的功能列按鈕都消失了

請安裝 <code>sudo apt-get install libqt4-svg</code>

安裝完之後請設定 compiler 以及 viewer

<code>options -> configure texstudio ->  Build -> Default Compiler -> XeLaTex</code> 


<code>options -> configure texstudio ->  Commands -> XeLaTex</code>

XeLatex 編譯出來是 pdf檔，需要比較多時間，適合最後腳交給老師的時候用

而用 latex 編譯出來是 dvi檔，比較快，適合撰寫的時候使用

用 pdf viewer 的後不會有問題

而如果是 dvi viewer，則可能會出錯

lubuntu 預設是用 evince 來開 dvi檔

而 evince 會抓不到 texlive 的檔案

所以要再安裝 texlive-binaries

可以下 <code>sudo apt-get install texlive-binaries</code>

如此就能成功編譯

參考連結：

- <a href="http://askubuntu.com/questions/400975/some-icons-symbols-in-texstudio-are-missing" target="_blank">http://askubuntu.com/questions/400975/some-icons-symbols-in-texstudio-are-missing</a>
-  <a href="http://tex.stackexchange.com/questions/54403/which-dvi-viewer-on-linux" target="_blank">http://tex.stackexchange.com/questions/54403/which-dvi-viewer-on-linux</a>