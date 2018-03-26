# 公式集

為簡化文章說明，將部分較為複雜的公式集合至此。

## 公司員工營利 {#company-employee-profit}

### 簡述 {#company-employee-profit-brief}

公司的每一位員工，都可以帶來一定的**基礎營利**，成長幅度由[公司評級](company.md#grade)決定。

除了基礎營利外，公司的每位員工都有一定機率**爆肝**，可額外再為公司帶來**爆肝加成營利**，以基礎營利的比例決定，比例的多寡由[公司評級](company.md#grade)決定。

將**基礎營利**加上**爆肝加成營利**乘以**爆肝員工人數**，即為該公司當日的**員工營利**。

### 詳細定義 {#company-employee-profit-detail}

定義**在職員工總人數**為 $$N$$。

定義**公司等級參數**為 $$t$$，由**公司評級**決定，對應如下：

| 公司評級 | 公司等級參數（$$t$$） |
| ------- | ------------------ |
| S 級、A 級 | 0.4 |
| B 級       | 0.3 |
| C 級       | 0.2 |
| D 級       | 0.1 |

定義**基礎營利**為 $$P_{base} = 3000 \times (0.9 + t)$$。

定義**爆肝機率**為 $$r = \text{min}(n, 30)\%$$，每位員工有 $$r$$ 的機率進行爆肝工作。

定義**爆肝員工人數**為一隨機變數 $$N_{boost} \sim B(n, r)$$，其中 $$B(n, p)$$ 為[二項式分佈](https://en.wikipedia.org/wiki/Binomial_distribution)。

定義**爆肝加成營利**為 $$P_{boost} = P_{base} \times t$$。

綜合以上，公司每日的**員工營利** $$P$$ 可寫為

$$
P = P_{base} + P_{boost} \times N_{boost}
$$

即**基礎營利**加上**爆肝加成營利**乘以**爆肝員工人數**。

## 公司挖礦機營利 {#company-mining-machine-profit}

### 詳細定義 {#company-mining-machine-profit-detail}

定義**總生產值**為 $$W$$，其值為挖礦機中所有石頭的**生產值加總**，若無石頭以 0 計。

定義**公司等級參數**為 $$t$$，由**公司評級**決定，對應如下：

| 公司評級 | 公司等級參數（$$t$$） |
| ------- | ------------------ |
| S 級    | 0.4 |
| A 級    | 0.3 |
| B 級    | 0.2 |
| C 級    | 0.1 |
| D 級    | 0   |

綜合以上，公司當季的**挖礦機營利** $$P$$ 可寫為

$$
P = 6300 \times \text{log}(W + 1) \times W^t
$$

## 公司 VIP 分數門檻 {#company-vip-score-thresholds}

定義**公司資本額**為 $$C$$，則 **Level 5 分數門檻**寫為

$$
T_5 = C \times (\frac{1487}{C})^{0.6}
$$

而 **Level 4 分數門檻** 至 **Level 1 分數門檻**則依序為

$$
\begin{aligned}
T_4 &= 0.8 \times T_5 \\
T_3 &= 0.6 \times T_5 \\
T_2 &= 0.4 \times T_5 \\
T_1 &= 0.2 \times T_5
\end{aligned}
$$

## 亂鬥排名獎勵 {#arena-ranking-awards}

定義**參賽總人數**為 $$N$$。

定義**所有參賽者投入金額總額**為 $$\sum P$$。

定義**存活獎勵變數**為
$$
A = 0.177 \times \frac{\sum P}{\text{ln}(N) + 0.57722 + \frac{1}{2 N}}
$$

則名次為第 $$i$$ 名者可以得到 $$\frac{A}{i}$$ 的**排名獎勵金**。

## 產品補貨釋出 {#product-replenishment}

定義**庫存數量**為 $$S$$。

定義**隨機釋出數**為一隨機變數 $$X \sim \text{Beta}(3, 7)$$，其中 $$\text{Beta}(\alpha, \beta)$$ 為 [Beta 分佈](https://en.wikipedia.org/wiki/Beta_distribution)。

則每次補貨的**釋出數量** $$N$$ 可寫為

$$
N = \text{min}(1, \lceil 0.1 \times S \times X \rceil)
$$

## 產品推薦票 {#product-vote-tickets}

若**上市公司總數**為 $$N$$，則每個玩家各別拿到的**推薦票總數** $$V$$ 為

$$
V = \text{min}(0, \lfloor\text{log}(N \times 18)\rfloor)
$$