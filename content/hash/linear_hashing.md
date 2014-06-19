Title: [hash] linear hashing
Slug: [hash]_linear_hashing
Category: hash
Author: Chris Yang

linear hashing 是一種 <font style="color:red;">dynamic hashing</font> 的方法

其儲存的欄位分為兩種 primary page, overflow page

並設N 為初始的 bucket 數

h_level (key) = key mod [N * 2 ^ N]

並存在一個 point Next 指向下一個要分割的 bucket

而 linear hashing 存在一個 utilization 的機制

超過 utilization 時則 split bucket



其演算法如下

    給定 N 為初始的 bucket 數, point Next 指向第0 個 bucket

    utilization is between 40% and 80%

    level 為 0

    1. 透過 hash function 來將 number insert 到 bucket 之中

    2. 檢查 utilization 是否超過 80%, 如果超過則 split next 指到的 bucket

    3. 重複步驟2 直到 utilization 降到 80% 以下

    如此可成功地將所有的number insert 到 bucket 之中



而split 的細節是

    將bucket 中的值去 mod 2 的倍數

    如果無法分開, 則挑選大一點的 2的倍數

    split 結束之後將 next 指向下一個bucket

    如果下一個 bucket >= N

    則將 next 歸0, 而 level +1

    要再insert 新的 number 時則使用新的 hash function 來 hash



<a href="{filename}/pdf/EDHashing.pdf" target="_blank">詳細教學與範例</a>


