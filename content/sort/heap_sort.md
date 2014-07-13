Title: [sort] heap sort
Date: 2014-06-22 00:00
Modified: 2014-06-22 00:00
Slug: [sort]_heap_sort
Category: sort
Author: Chris Yang

heap sort 使用了 heap 來幫助我們做sort 的工作

時間複雜度為 <code>O(n logn)</code>

為穩定排序法

核心概念為運用heap 的特性

假設我們有一個 size 為 n 的 heap

每次將root 與heap 的最後一個位置交換

然後再執行一次 size 為 n-1 的 <font style="color:red;">heapify()</font>

重複此動作直至所有元素都被排序完為止



在實作的部分

我們習慣將存data 的陣列的第0個位置空出來

從第1個位置開始存

這樣才能符合 heap 的特性

<a href="https://github.com/yljh21328/code_example/blob/master/SORT/heap_sort/heap_sort.java" target="_blank">heap sort – JAVA</a>

