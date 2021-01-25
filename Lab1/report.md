# 兩個神經元和四個神經元比較:
我是先作兩個神經元的訓練,將測試結果帶入測試資料都會跑出相符的結果,但再四個神經元訓練,就不是這樣的,Dataset 1 及 Dataset 2 三個性質所形成帶入訓練出的 weight 和 bias,帶入測試資料中,會有產生出不在任何一分類的結果。我覺得是因為四個神經元較能呈現出更多元的結果,資料有可能介於多種分類之間,所以顯示出的結果才不在任一分類上,這樣的好處是,我們可以更易於分析是否資料不夠豐富,或是需要調整參數做應變。
# 訓練資料和測試資料:
得不出結果還有另一種看法,訓練出的 weight 和 bias 是根據訓練資料所產生而成的,測試資料如果和訓練資料有差距,就會產生不出結果,除了有可能是資料是否充足問題,或是資料會有界於多種分類之間外,也有可能是少許測試資料可能在收集時發生錯誤,如果是這後這一種情況的話,就要重新收集資料,花費許多時間成本,必須避免這種情形。
# Learning rate:
我在寫程式時會一直調整 Learning rate,當中最讓我深刻的應該是 Learningrate 和測試結果, Learning rate 只差 $0.1$ 或更小,有些測試資料就從找到結果變成找不到,這代表著如果我沒有好好調的話,就可能會得出偏差很大的結果。