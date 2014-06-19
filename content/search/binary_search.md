Title: [search] binary search
Slug: [search]_binary_search
Category: search
Author: Chris Yang

binary search 是一種用於事先排序好的資料的搜尋演算法

算是 <font style="color:red;">divide and conquer</font> 的變形 (少了 merge 的步驟)

核心概念於訂定三個 index : low, mid, high

如果要找的 key 大於 data[mid], 則搜尋右半邊

如果小於 data[mid] 則搜尋左半邊

否則回傳mid 的位置

一直找下去

如果 high < low 則代表找尋不到

因其每次可以prune 掉一半的資料

所以其時間複雜度為 O(n log n)

<a href="https://github.com/yljh21328/code_example/blob/master/SEARCH/binary_search/binary_search.java" target="_blank">binary search – JAVA</a>
