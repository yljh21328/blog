Title: [sort] quick sort
Slug: [sort]_quick_sort
Category: sort
Author: Chris Yang

quick sort 是一個內部排序法

平均時間複雜度為 <code>O(n logn)</code>

worst case 的時間複雜度為 O(n^2)

採取的是 <font stlye="color:red;">divide and conquer</font> 的模式來解決問題

核心概念是先設整個序列的第一個值為K

然後從左至右找到一個比K 大的元素 Ki

並從右到左找到一個比K小的元素Kj

找到後就彼此交換

直到 i < j 時

此時再將 Kj 與 K 的位置交換

結束這回合

此時便能決定K的位置

然後再利用divide and conquer 來解決左邊與右邊尚未解決的subsequence

<a href="https://github.com/yljh21328/code_example/blob/master/SORT/quick_sort/quick_sort.java" target="_blank">quick sort – JAVA</a>


