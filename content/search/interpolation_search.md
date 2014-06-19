Title: [search] interpolation search
Slug: [search]_interpolation_search
Category: search
Author: Chris Yang

interpolation search 為 binary search 的改良版

適合用在資料平均分佈的狀況下

其內插法公式為

mid = low + ((key – data[low]) / (data[high] – data[low])) * (high – low)

而其餘的搜尋步驟則與 binary search 差不多



平均而言其時間複雜度優於 <code>O(log n)</code>



<a href="https://github.com/yljh21328/code_example/blob/master/SEARCH/interpolation_search/interpolation_search.java" target="_blank">interpolation search – JAVA</a>
