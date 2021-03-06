# 最萌亂鬥大賽

每**兩個商業季度**會舉辦一次最萌亂鬥大賽，這是一個以趣味性為主的賭搏活動。

## 報名 {#join}

每屆大賽的報名截止時間為**商業季度結束前 24 小時**，經理人可以為自己管理的公司報名參賽。

## 投注與屬性值 {#investigation-and-attributes}

公司在報名之後，預設會取得 **100** 點 HP、**10** 點 SP、**20** 點 ATK、**5** 點 DEF、**0** 點 AGI 屬性。直到舉辦最萌亂鬥大賽的**商業季度結束前**，所有人都可以自由的對已報名的公司的個別屬性進行投注。每投資 **$200** 可提升 **1** 點 HP，每投資 **$1,000** 可提升 **1** 點 SP，每投資 **$1,000** 可提升 **1** 點 ATK，每投資 **$1,000** 可提升 **1** 點DEF，每投資 **$1,000** 可提升 **1** 點 AGI。

所有參賽者的屬性點現況將會即時顯示於最萌亂鬥大賽的資訊頁當中，先投注少量金錢在敵人身上以令其吸引火力也是策略的一種。

若是在大賽正式開始時，總投注金額**未達 $10,000** 者，將被**取消參賽資格**，從參賽名單中刪除，而投注金額也將**全數退還**給原投注人。

對最萌亂鬥大賽參賽者的投注是**無法主動取回**的，大賽獲利也**不會**依照投注比例進行分紅，請謹慎投注。

## 決策 {#strategy-decision}

在報名亂鬥大賽之後，經理人可自由設定參賽公司的**特殊攻擊消耗點數**、至多三個的**普通攻擊招式名稱**與至多三個的**特殊攻擊招式名稱**。

設定**特殊攻擊消耗點數**時，不可以超過角色當前的 **SP 值總量**，也不可以超過 **10**。

在亂鬥大賽報名截止之後，經理人將可以決定該公司的**優先攻擊順序**，對所有自身之外參賽者進行排序。

## 亂鬥程序

在商業季度結束、進行公司分紅之前時，會先進行最萌亂鬥大賽的運算。

所有參賽者將會依據**對 AGI 的投注額**進行排序，**AGI 越高者越先行動**，當AGI相同時，公司上市日期較早者將會優先行動。

參賽者行動時，會依據其經理人設定的**優先攻擊順序**挑選尚存活的攻擊目標，一次行動只能攻擊一個目標。

參賽者行動時，若其殘餘 SP 大於經理設定的**特攻消耗數值**，則會進行**特攻檢定**：系統將決定一個 1 到 10 之間的隨機數字，若經理設定的特攻消耗數值大於或等於該數字，則角色將失去等同特攻消耗數值設定值的 SP 並發動**特殊攻擊**，否則只會發動普通攻擊。

若攻擊者發動的是普通攻擊，則需要進行**命中檢定**以決定是否擊中防禦者，依照攻防方的數值決定攻擊方的**命中率**（[公式](formulas.md#arena-hit-rate)）。若是此次成功命中防禦者，將根據攻擊者與防禦者的數值，計算造成的**傷害**（[公式](formulas.md#arena-damage)），並從防禦方的 HP 扣除。

若攻擊者發動的是**特殊攻擊**，則該次攻擊**必定命中**，且計算傷害時**防禦方 DEF 以三分之一計算**。

若防禦者在攻擊者攻擊之後，**殘餘HP小於或等於0，則視為落敗**。攻擊者將獲得**防禦者各屬性的總投注金額**數量再加上 **$5,000** 的收益，而已經落敗的參賽者將無法行動。

當所有存活的參賽者結束行動後，一個回合結束，所有尚且存活的參賽者將**恢復 1 點SP**。

## 排名與收益

亂鬥中，第一位陣亡者為最後一名，第二位陣亡者為倒數第二名，依此類推。當存活者**剩下一位**時，存活者為第一名，且大賽結束。

若存活者剩下多位但戰鬥已**超過 1000 回合**時，大賽也會結束，剩餘存活者將**依據殘餘 HP 進行排名**，HP相同者將以行動順序決定先後。

所有參賽者除了各自的擊倒獎勵之外，亦將依照存活排名獲得**排名獎勵**（[公式](formulas.md#arena-ranking-awards)）。

參賽者的參賽總收益將直接算入該公司在當季度的本季營利中，並在之後的商業季度結算依照規則對經理人與董事分紅。跟投注者沒有直接關係。