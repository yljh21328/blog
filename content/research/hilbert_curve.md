Title: [research] Hilbert Curve
Slug: [research]_hilbert_curve
Category: research
Author: Chris Yang

令 N = 2^n

在一個 size 為 N x N 的二維空間中

Hilbert curve 會遞迴地將我們的空間切成四個相同size 的 blocks

而每一個 block 我們都會給一個 0 ~ N^2 -1 的number

<img src="{filename}/images/hilbert_curve.png" />

舉例來說

order n = 1 時我們可以得到一串分別是 0 ~ 3 的數字

而 order n = 2 則是由 order n = 1 演化而來

只要將order n = 1 的第一個 block 與最後一個 block 做 reflection 跟 rotation 即可得到結果

依此類推

order n = 3 是由 order n = 2 演化而來, 做的是相似的 reflection 與 rotation

