Title: [research] The Bucket Numbering Scheme
Slug: [research]_the_bucket_numbering_scheme
Category: research
Author: Chris Yang

一個空間上的物件可以是任意形狀

而通常我們會取一個 bounding rectangle 來表示這個物件

而坐標可利用 Xl, Xr, Yb, Yt四個屬性來定義

在此我們用 L(Xl,Yb) 與 U(Xr,Yt) 來表示一個物件

在 Bucket Number Scheme 裡面我們將一個 Bucket 以 0 或 1 來表示

也稱作 <font style="color:red;">DZ expression</font>

表示的規則有兩點：

* 在x軸中的0表示左半部, 1表示右半步。而在y軸中0表示下半部, 1表示上半部

* 越左邊的bit 代表越前面的binary division, 越後面的bit 代表越裡面的division

<img src="{filename}/images/dz_expression.png" />

以圖中的例子

舉例來說 0010* 表示的是

00代表的是整個區塊裡面的左半部及下半部

10代表的是左半部及下半部中，右半部及下半部

以此類推。

而在此我們也會使用 Max_bucket 來記錄所有bucket 中最大的 bucket number

<img src="{filename}/images/peano_curve.png" />

在 Fig.6(a) 中我們將 binary form 轉成 decimal form

而在 Fig.6(b) 中我們可以依照順序劃線來得到 N-order peano curve

