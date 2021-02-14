### Social Distancing II

由于高传染性的牛传染病 COWVID-19 的爆发，Farmer John 非常担忧他的奶牛们的健康。

尽管他尽了最大努力使他的 $N$ 头奶牛们（$1 \leq N \leq 1000$）践行“社交距离”，还是有许多奶牛不幸染上了疾病。编号为 $1 \ldots N$ 的奶牛们分别位于一条长直道路上的不同位置（相当于一维数轴），奶牛 $i$ 位于位置 $x_i$。Farmer John 知道存在一个半径 $R$，任何与一头被感染的奶牛距离不超过 $R$ 单位的奶牛也会被感染（然后会传染给与其距离 $R$ 单位内的奶牛，以此类推）。

不幸的是，Farmer John 并不确切知道 $R$ 的值。他只知道他的哪些奶牛被感染了。给定这个数据，求出起初感染疾病的奶牛的最小数量。



#### 输入格式（文件名：socdist2.in）：

输入的第一行包含 $N$。以下 $N$ 行每行用两个整数 $x$ 和 $s$ 描述一头奶牛，其中 $x$ 为位置（$0 \leq x \leq 10^6$），$s$ 为 0 表示健康的奶牛，1 表示染病的奶牛，并且所有可能因传播而染病的奶牛均已染病。



#### 输出格式（文件名：socdist2.out）：

输出在疾病开始传播之前已经得病的奶牛的最小数量。



#### 输入样例：

```
6
7 1
1 1
15 1
3 1
10 0
6 1
```

#### 输出样例：

```
3
```

在这个例子中，我们知道 $R < 3$，否则位于位置 7 的奶牛会传染给位于位置 10 的奶牛。所以，至少 3 头奶牛初始时已被感染：位于位置 1 和 3 的两头奶牛中的一头，位于位置 6 和 7 的两头奶牛中的一头，以及位于位置 15 的奶牛。

#### 思路分析