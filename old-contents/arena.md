# 最萌亂鬥大賽說明
1. 每<font color="#A3A3FF">兩個商業季度</font>會舉辦一次最萌亂鬥大賽，這是一個以趣味性為主的賭搏活動。
1. 報名與投注：
    1. 直到舉辦最萌亂鬥大賽的商業季度結束前一天（也就是經理人選舉活動之前），所有已上市公司皆可以報名參賽。
    <font color="#A3A3FF">1</font>. 所有報名公司預設會取得<font color="#A3A3FF">50</font>點HP、<font color="#A3A3FF">5</font>點SP、<font color="#A3A3FF">1</font>點ATK、<font color="#A3A3FF">0</font>點DEF、<font color="#A3A3FF">0</font>點AGI屬性。
    <font color="#A3A3FF">1</font>. 直到舉辦最萌亂鬥大賽的商業季度結束前，所有人都可以自由的對已報名的公司的個別屬性進行投注。每投資<font color="#A3A3FF">$200</font>可提升<font color="#A3A3FF">1</font>點HP，每投資<font color="#A3A3FF">$1000</font>可提升<font color="#A3A3FF">1</font>點SP，每投資<font color="#A3A3FF">$1000</font>可提升<font color="#A3A3FF">1</font>點ATK，每投資<font color="#A3A3FF">$1000</font>可提升<font color="#A3A3FF">1</font>點DEF，每投資<font color="#A3A3FF">$1000</font>可提升<font color="#A3A3FF">1</font>點AGI
    <font color="#A3A3FF">1</font>. 所有參賽者的屬性點現況將會即時顯示於最萌亂鬥大賽的資訊頁當中，先投注少量金錢在敵人身上以令其吸引火力也是策略的一種。
    1. 若是在<font color="orange">大賽正式開始時</font>，總投注金額<font color="orange">未達$10000</font>者，將被<font color="red">取消參賽資格</font>，從參賽名單中刪除，而投注金額也將全數退還給原投注人。
    1. 對最萌亂鬥大賽參賽者的投注是<font color="red">無法主動取回</font>的，大賽獲利也<font color="red">不會</font>依照投注比例進行分紅，請謹慎投注。
1. 經理人決策：
    1. 在報名亂鬥大賽之後，所有經理人皆可自由設定參賽公司的「特殊攻擊消耗點數」、至多三個的「普通攻擊招式名稱」與至多三個的「特殊攻擊招式名稱」。
    1. 設定「特殊攻擊消耗點數」時，不可以超過角色當前的SP值總量，也不可以超過10。
    1. 在亂鬥大賽報名截止之後（經理人選舉活動之後），新任經理人將可以決定該公司的「優先攻擊順序」，對所有自身之外參賽者進行排序。
1. 亂鬥程序：
    1. 在商業季度結束、進行公司分紅之前時，會先進行最萌亂鬥大賽的運算。
    1. 所有參賽者將會依據對<font color="#A3A3FF">AGI</font>的投注額進行排序，AGI越高者越先行動，當AGI相同時，<font color="#A3A3FF">公司上市日期較早者</font>將會優先行動。
    1. 參賽者行動時，會依據其經理人設定的「優先攻擊順序」挑選尚存活的攻擊目標，一次行動只能攻擊一個目標。
    1. 參賽者行動時，若其<font color="#A3A3FF">殘餘SP</font>大於經理設定的「<font color="#A3A3FF">特攻消耗數值</font>」，則會進行特攻檢定。系統將決定一個<font color="#A3A3FF">1到10之間</font>的隨機數字，若經理設定的「特攻消耗數值」大於或等於該數字，則角色將失去<font color="#A3A3FF">等同特攻消耗數值設定值</font>的SP並發動特殊攻擊，否則只會發動普通攻擊。
    1. 若攻擊者發動的是普通攻擊，則需要進行命中檢定以決定是否擊中防禦者。系統將決定一個<font color="#A3A3FF">1到100之間</font>的命中隨機數字，其加上攻擊者AGI後大於等於防禦者的AGI則命中成功，否則視為攻擊落空。<font color="red">但是</font>若命中隨機數字<font color="#A3A3FF">大於95</font>，則無論攻防方的AGI差距多少都必然會命中。
    1. 若攻擊者發動的是普通攻擊，在命中防禦者後，將造成<font color="#A3A3FF">攻擊者ATK減去防禦者DEF</font>的傷害，<font color="red">但</font>只要攻擊命中，最小也會造成<font color="#A3A3FF">1</font>點傷害。
    1. 若攻擊者發動的是特殊攻擊，那該次攻擊將無視AGI、DEF，必然對防禦者造成等同於<font color="#A3A3FF">攻擊者ATK數值</font>的傷害。
    1. 若防禦者在攻擊者攻擊之後，殘餘HP小於或等於0，則視為落敗。攻擊者將獲得<font color="#A3A3FF">防禦者各屬性的總投注金額數量</font>再加上<font color="#A3A3FF">$5000</font>的收益。
    1. 已經落敗的參賽者將無法行動。
    1. 當所有存活的參賽者結束行動後，一個回合結束，所有尚且存活的參賽者將恢復<font color="#A3A3FF">1</font>點SP。
1. 排名與收益：
    1. 亂鬥中，第一位陣亡者為最後一名，第二位陣亡者為倒數第二名，依此類推。
    1. 當存活者<font color="#A3A3FF">剩下一位</font>時，存活者為第一名，且大賽結束。
    1. 若存活者剩下多位但戰鬥已超過<font color="#A3A3FF">1000</font>回合時，大賽也會結束，剩餘存活者將依據殘餘HP進行排名，HP相同者將以行動順序決定先後。
    1. 所有參賽者除了各自的擊倒獎勵之外，亦將依照存活排名獲得排名獎勵。存活獎勵變數為<font color="#A3A3FF">0.177</font>×<font color="#A3A3FF">所有參賽者的總投入金額</font>÷（<font color="#A3A3FF">ln(所有參賽者數量)</font>＋<font color="#A3A3FF">0.57722</font>＋（1÷<font color="#A3A3FF">兩倍參賽者數量</font>））。第一名可以獲得獎勵變數除以一的排名獎勵金，第二名可以獲得獎勵變數除以二的排名獎勵金，依此類推。
    1. 參賽者的參賽總收益將直接算入該公司在當季度的本季營利中，並在之後的商業季度結算依照規則對經理人與董事分紅。跟投注者<font color="red">沒有</font>直接關係。