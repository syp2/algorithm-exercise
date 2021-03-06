# Counting Sort

計數排序，顧名思義，就是對待排序陣列按元素進行計數。使用前提是需要先知道待排序陣列的元素範圍，將這些一定範圍的元素置於新陣列中，新陣列的大小爲待排序陣列中最大元素與最小元素的差值。

維基上總結的四個步驟如下：

1. 定新陣列大小——找出待排序的陣列中最大和最小的元素
2. 統計次數——統計陣列中每個值爲i的元素出現的次數，存入新陣列C的第i項
3. 對統計次數逐個累加——對所有的計數累加（從C中的第一個元素開始，每一項和前一項相加）
4. 反向填充目標陣列——將每個元素i放在新陣列的第C(i)項，每放一個元素就將C(i)減去1

其中反向填充主要是爲了避免重復元素落入新陣列的同一索引處。

## Reference

- [計數排序 - 維基百科，自由的百科全書](http://zh.wikipedia.org/wiki/%E8%AE%A1%E6%95%B0%E6%8E%92%E5%BA%8F) - 中文版的維基感覺比英文版的好理解些。
- [Counting Sort Visualization](https://www.cs.usfca.edu/~galles/visualization/CountingSort.html) - 動畫真心不錯~ 結合著看一遍就理解了。
