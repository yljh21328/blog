Title: [sort] merge sort
Slug: [sort]_merge_sort
Category: sort
Author: Chris Yang

merge sort 是一個 external sort

其時間複雜度為 <code>O(n logn)</code>

適合合併多個檔案並排序

如果有兩個檔案要做排序

核心概念是先分別對這倆個檔案做內部排序

之後再分別用指標指著這兩個檔案

依序讀入後比較

並將較小的元素給存到一個新的 sequence當中

而該檔案繼續讀下一個元素

直到讀完為止

而如果其中一個檔案先讀完

則直接將另外一個檔案的內容依序讀入sequence

直至兩個檔案都讀完為止

如此我們就可以得到一個排序過後的sequence

<a href="https://github.com/yljh21328/code_example/tree/master/SORT/direct_merge_sort" target="_blank">直接merge – JAVA</a>

<a href="https://github.com/yljh21328/code_example/tree/master/SORT/complete_merge_sort" target="_blank">分割檔案後再merge – JAVA</a>

