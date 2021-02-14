### Mad Scientist

Farmer John 的远房亲戚 Ben 是一个疯狂的科学家。通常这会在家庭聚会时造成不小的摩擦，但这偶尔也会带来些好处，尤其是当 Farmer John 发现他正面对一些有关他的奶牛们的独特而不寻常的问题时。

Farmer John 当前正面对一个有关她的奶牛们的独特而不寻常的问题。他最近订购了 $N$ 头奶牛（$1 \leq N \leq 1000$），包含两种不同品种：荷斯坦牛和更赛牛。他在订单中用一个长为 $N$ 的字符串来指定奶牛，其中的字符为 H（表示荷斯坦牛）或 G（表示更赛牛）。不幸的是，当这些奶牛到达他的农场，他给她们排队时，她们的品种组成的字符串与原先的不同。

我们将这两个字符串称为 $A$ 和 $B$，其中 $A$ 是 Farmer John 原先想要的品种字符组成的字符串，$B$ 是他的奶牛们到达时组成的字符串。Farmer John 并没有简单地检查重新排列 $B$ 中的奶牛是否能得到 $A$，而是请他的远房亲戚 Ben 利用他的科学才华来解决这一问题。

经过数月的研究，Ben 发明了一台不同寻常的机器：奶牛品种转换机3000，能够选择任意奶牛组成的子串并反转她们的品种：在这个子串中的所有 H 变为 G，所有 G 变为 H。Farmer John 想要求出将他当前的序列 $B$ 变为他本来订购时想要的 $A$ 需要使用这台机器的最小次数。然而，Ben 的疯狂的科学家技能并不会处理开发奇异机器以外的事，所以你需要帮助 Farmer John 解决这个计算难题。



#### 输入格式（文件名：breedflip.in）：

输入的第一行包含 $N$，以下两行包含字符串 $A$ 和 $B$。每个字符串均包含 $N$ 个字符，字符均为 H 和 G 之一。



#### 输出格式（文件名：breedflip.out）：

输出将 $B$ 变为 $A$ 需要使用机器的最小次数。



#### 输入样例：

```
7
GHHHGHH
HHGGGHH
```

#### 输出样例：

```
2
```

首先，FJ 可以仅改变第一个字符组成的子串，将 $B$ 变为 GHGGGHH。然后，他可以改变由第三和第四个字符组成的子串，得到 $A$。当然，还存在其他有效的执行两次操作的方案。