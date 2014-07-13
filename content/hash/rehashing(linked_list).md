Title: [hash] rehashing
Date: 2014-06-05 00:00
Modified: 2014-06-05 00:00
Slug: [hash]_rehashing
Category: hash
Author: Chris Yang

rehashing 的概念是在hash 的過程中如果遇到 collision 與 overflow

則再改用另外一種 hash function 來hash

而在此我們使用 <font style="color:red;">linked list</font> 來解決 collision 與 overflow 的問題

透過不斷的往後串即可

<a href="https://github.com/yljh21328/code_example/blob/master/HASH/rehashing/rehashing.java" target="_blank">rehashing – JAVA</a>



而下面的範例是加上搜尋的功能

<a href="https://github.com/yljh21328/code_example/blob/master/HASH/rehashing_search/rehashing_search.java" target="_blank">rehashing with search – JAVA</a>
