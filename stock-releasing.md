# 股份釋出

## 初始釋股 {#initial-offering}

在公司成立之初，將依照投資人投入的金額，進行**初始釋股**，此時將以**初始股價**乘上**初始釋股數**作為公司的**初始資本額**。

詳細的計算方式請參見[新創成功時的說明](foundation.md#foundation-success)。

## 高價釋股 {#high-price}

每隔 **3 ~ 6 小時**的隨機時間，系統將觸發**高價釋股**程序，當公司滿足以下條件，即會進行股份釋出：

* [**最後價格**](company.md#price)需**大於等於**市場的**[高價公司門檻](company.md#high-low-price-thresholds)**
* **不存在**任何**[系統釋股賣單](stock-trading#system-sell-orders)**

釋出股份時將產生[系統釋股賣單](stock-trading#system-sell-orders)，其**數量**為 **1 ~ 總釋股數的平方根**之間的隨機整數，**價格**則為當下的[**漲停價格**](stock-trading#price-limits)。

## 低成交量釋股 {#low-volume}

每隔 **24 ~ 48 小時**的隨機時間，系統將觸發**低成交量釋股**程序，當公司**最近 24 小時成交量的十倍小於所有漲停價以上買單的未成交量總和**，即會進行股份釋出。

釋出股份時將產生[系統釋股賣單](stock-trading#system-sell-orders)，其**數量**為 **1 ~ 所有漲停價以上買單的未成交量總和的一半**之間的隨機整數，**價格**則為當下的[**漲停價格**](stock-trading#price-limits)。
