Title: [linux] 修改 apt 的 mirror site
Slug: [linux]_apt_mirror_site
Category: linux
Author: Chris Yang

安裝 ubuntu 預設的更新源是 <code>tw.archive.ubuntu.com</code>

這個source 又慢又不穩定

利用以下的步驟就可以幫 ubuntu 換一個最佳的更新源


- cp /etc/apt/sources.list /etc/apt/sources.list.backup

- sudo /usr/bin/software-properties-gtk

- Tab 選 "Ubuntu軟體"

- 下載自選擇 ""其它"

-  然後跑 "選擇最佳的伺服器"

跑完就有最佳的更新源了

參考來源：<a href="http://blog.longwin.com.tw/2011/02/ubuntu-mirror-site-repository-2011/">Ubuntu Linux 挑選最佳的 Mirror Site (APT Repository) </a>
