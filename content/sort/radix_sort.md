Title: [sort] radix sort
Date: 2014-06-26 00:00
Modified: 2014-06-26 00:00
Slug: [sort]_radix_sort
Category: sort
Author: Chris Yang

radix sort 是一個不需要兩兩比較元素的一種排序法

其核心概念是透過分配每一個元素到適當的位置

我們可以先從最低位數開始比較或從最高位數開始比較都可以

假設我們從最低位數開始比較

依照所比對到的元素該位數的值

依序放置到相對應的位置

最後整個比較完之後依序取出即可得到正確答案



時間複雜度為 <code>O(n log_p  k)</code>

p 為資料字元數

缺點是需要花費大量的額外空間來暫存資料

若n 很大, 但是p 固定或很小

則此演算法十分有效率



<a href="https://github.com/yljh21328/code_example/blob/master/SORT/radix_sort/radix_sort.java" target="_blank">radix sort – JAVA</a>
