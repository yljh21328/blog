Title: [search] fibonacci search
Slug: [search]_fibonacci_search
Category: search
Author: Chris Yang


fibonacci search 跟 binary search 一樣都是使用二分法來進行切割範圍和搜尋

不同的是 fibonacci 是用 <font style="color:red;">fibonacci number</font> 來切割

也就是說我們會先建立一個 fibonacci tree

然後再依照此 tree 來做search

示意圖 – <a href="http://puremonkey2010.blogspot.tw/2010/12/blog-post.html" target="_blank">來源</a>


<img src="{filename}/images/fibonacci_tree.jpg" />




fibonacci tree 的 root 是由資料個數 n 決定的

先利用 Fib(k+1) >= n + 1

來決定 k

再以Fib(k) 當作root 的值

而其左子樹為 (k – 1) 階Fibonacci tree

右子樹為 (k-2) 階 Fibonacci tree

依此類推可以建立完整的 Fibonacci tree



更多詳細資料可參考 – <a href="http://puremonkey2010.blogspot.tw/2010/12/blog-post.html" target="_blank">程式扎記</a>
