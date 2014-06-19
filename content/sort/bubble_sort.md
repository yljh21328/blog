Title: [sort] bubble sort
Slug: [sort]_bubble_sort
Category: sort
Author: Chris Yang

bubble sort 是一種 internal sort

適合資料量小或已經有初步排序的資料使用

其 worst case 為 <code>O(n^2)</code>

如果是要由小排到大

核心概念是由前往後兩兩比對，若前者大於後者則交換

並由較大者繼續與後面的元素兩兩比對。

每scan一次能確定一個元素的最後位置

<a href="https://github.com/yljh21328/code_example/blob/master/SORT/traditional_bubble_sort/bubble_sort.java" target="_blank">傳統版 - JAVA</a>

<a href="https://github.com/yljh21328/code_example/blob/master/SORT/better_bubble_sort/bubble_sort.java" target="_blank">改良版 - JAVA</a>

在改良版的bubble sort 裡加入了 flag 來判斷該次 scan 有沒有做 swap

如果沒有則不需要額外的 scan
