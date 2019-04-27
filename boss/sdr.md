#Existence of SDRS

<font color="red" style="font-weight: bold;font-size:x-large;">Defn:</font> 

![](/assets/sdr1.png)
- - -

集族$$\bold{A}(A_1,A_2,A3,...,A_n)$$ 设k是满足1$$\leqslant$$k$$\leqslant$$n的整数 为了使$$\bold{A}$$有一个SDR，<font color="red" style="font-weight: bold">族A的每k个集合的并集必须至少包含k个元素</font>

如果不是这样， 比如$$A_1,A_2,...,A_k$$ 它们合起来包含的元素个数小于k，即

$$A_1\bigcup A_2\bigcup A_3 ... \bigcup A_k = F$$ 其中$$|F| < k$$

这时，这k个集合$$A_1,A_2,...,A_k$$中的每一个集合的代表一定来自于集合$$F$$的元素。因为$$F$$的元素个数小于$$k$$，因此，根据pigeonhole principle 这k个集合中至少有两个集合有相同的代表。因此不存在SDR

![](/assets/sdr2.png)
- - -

<font color="red" style="font-size: x-large">MC不仅是SDR存在的必要条件而且还是充分条件</font>

![](/assets/sdr3.png)

![](/assets/sdr4.png)

![](/assets/sdr5.png)

- - - 

**证明分为两个互补的情况(条件限定在1$$\leqslant$$k$$\leqslant$$n-1) tight case和spare-room case**

* tight case是存在 k个集合的并集刚好有k个元素，将n个元素划分为k个集合和剩下的n-k个集合，由于k的范围，这个划分的两个集族均非空，k个集合的集族明显有SDR(因为是原集族的子集)，而另外一个集族 是将剩下的集合中每个集合去除前面k个集合并起来的所有元素，是一个构造的集族而非原集族A的子集，所以要对这个集族证明MC条件成立，由归纳法就可以知道划分出的两个集族都有SDR，又这两个集族内容不相同，所以两个SDR可以合并成集族A的SDR

* spare-room case是1$$\leqslant$$k$$\leqslant$$n-1时每一个k个集合的子集并起来元素都至少为k+1，条件比tight case更强，证明的方法就是$$A_1,A_2,A_3,...,A_n-1$$的每个集合减去$$A_n$$的代表$$e_n$$ 然后证明$$A_1,A_2,A_3,...,A_n-1$$满足MC条件 由归纳法可得$$A_1,A_2,A_3,...,A_n-1$$ 有SDR，由于$$A_1,A_2,A_3,...,A_n-1$$中没有$$e_n$$，所以拼起来以后可以得到原集族A的一个SDR

**综合两种情况 由归纳法就可以证明**
- - -

下面是回答一个关键问题：

<font color="red" style="font-size: x-large">拥有SDR的子族中集合的最大数量是多少</font>

![](/assets/sdr6.png)

