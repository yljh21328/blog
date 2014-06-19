Title: [sort] insertion sort
Slug: [sort]_insertion_sort
Category: sort
Author: Chris Yang

insertion sort 是一個 internal sort

其worst case 的時間複雜度為 <code>O(n^2)</code>

如果要由小排到大

核心概念為逐次檢查元素與其之前元素的大小

如果比之前的元素小則將前面的元素往後推

直到找到正確的位置為止

因為在 scan 的過程中會發生多次的搬移

所以如果以 linked list 來實作的話會快很多

<a href="https://github.com/yljh21328/code_example/blob/master/SORT/insertion_sort/insertion_sort.java" target="_blank">Array版 – Java</a>
