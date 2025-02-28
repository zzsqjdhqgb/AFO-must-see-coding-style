# very valuable AFO experience

-   DFS 搜索一张图，直接使用 `gr[u].size()` 判断儿子数量，完全忘记有个东西叫自环

-   $O(1)$ LCA 并没有想起来要给深度最小的点再套一个 `fa[]`

-   线段树访问了第 0 位，然而传入的范围是从 1 开始的

-   `vector` 建双向边，然后 `u` 和 `v` 写错了
    对着核心代码调了很久很久，并没有看一眼输入输出写没写对

    ```cpp
    gr[u].push_back(v);
    gr[v].push_back(v);
    ```

-   线段树维护区间的 `min` 和 `max`，相当悲剧的写反了

    ```cpp
    ma[rt] = max(ma[rt], v);
    mi[rt] = max(mi[rt], v);
    ```

-   曾经不熟练 `KMP` 的时候，误认为单个字符的 `border` 是 1，于是所有串的 `border` 都被计算成了它本身

-   FHQ-Treap，如果多个相同的值存在同一个点里，不能用 split 来实现 k-th

-   因为不会，所以打了一堆部分分，然而忘记在每一个特判后面写 `return 0;`，把所有特殊性质全跑了一遍