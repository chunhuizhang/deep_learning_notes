

> transformer/bert 中因为有了 attention 机制的存在（`attention is all you need`，注意力机制成为其最重要的算子），而 attention 均可通过矩阵乘法实现，底层计算上 transformer/bert 最重要的运算即是矩阵乘法运算。

## 1. 浮点数运算

- 一个 $A_{m\cdot n}$ 的矩阵与一个 $B_{n\cdot p}$ 的矩阵相乘
    - $A\cdot B=C_{m\cdot p}$ 矩阵 $C$ 的 entry 数量为 $m\cdot p$；
    - 对于每一个 entry，其浮点数运算为 $n$ 次乘法，$n-1$次加法，浮点数运算为 $2n-1$
    - 因此其浮点数运算的数量为 $mp(2n-1)\approx 2mnp$
    
    - 如果 $A_{n\cdot n}\cdot B_{n\cdot n}=C_{n\cdot n}$，则其浮点数运算量为 $2n^3$
 