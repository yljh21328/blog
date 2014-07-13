Title: [linux] ubuntu 架設 ftp (使用vsftp)
Date: 2014-06-11 00:00
Modified: 2014-06-11 00:00
Slug: [linux]_ftp_(vsftp)
Category: linux
Author: Chris Yang


* 安裝指令:

    <code>sudo apt-get install vsftpd</code>

* 確認是否安裝成功:

    <code>netstat -tul | grep ftp</code>


    如果有出現 <code>Listen</code> 即為安裝成功

* 修改設定檔:

    <code>sudo vim /etc/vsftpd.conf</code>

        :::bash
        #接受匿名用戶
        anonymous_enable=NO
        #接受本地用戶
        local_enable=YES
        #可以上傳(全局控制).若想要匿名用戶也可上傳則需要設置
        #anon_upload_enable=YES,若想要匿名用戶可以建立目錄
        #則需要anon_mkdir_write_enable=YES.
        #這裡禁止匿名用戶上傳,所以不設置這兩項.
        write_enable=YES

* 修改完記得重新啟動:

    <code>sudo /etc/init.d/vsftpd restart</code>

<a href="http://blog.udn.com/nigerchen/2261345" target="_blank">參考來源</a>

