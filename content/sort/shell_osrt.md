Title: [sort] shell sort
Slug: [sort]_shell_sort
Category: sort
Author: Chris Yang


shell sort 是 insertion sort 的改良版

average case 的時間複雜度為 <code>O(n ^ 3/2)</code>

屬於internal sort, 穩定排序

目的是為了減少 insertion sort 的搬移次數

其核心概念為將要排序的數依<font color="red">劃分數</font>來分群

最簡單的做法就是設定劃分數為2

因此如果我們有8筆資料的話我們就可以分成4群  (4 = 8 / 2)

而分別做完一次 insertion sort 之後

再將劃分數 double, 也就是變成4

此時我們只會劃分為2群 (2 = 8 / 2 / 2)

依此類推

直到分群結束為止

而劃分的方式是採取間隔的方式來取元素

舉例來說如果我們有8個元素

63, 92, 27, 36, 45, 71, 58, 7

因此我們亦開始會得到 {63,45}, {92,71}, {27,58} 以及{36,7} 4 群

依此類推

如此我們就可以減少insertion sort 的搬移次數

<a href="https://github.com/yljh21328/code_example/blob/master/SORT/shell_sort/shell_sort.java" target="_blank">Array版 – JAVA</a>
