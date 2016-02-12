進入Linux Bridge之前先介紹名詞

Bridge

Interface

hairpin

Ageing Time(生命週期)

    Linux Bridge封包生命週期單位為"秒鐘":
    
        從目的地接收"封包"之後會將該時間儲存至封包中。在轉發過程中將定時被檢查有無超時，以確保它們不會永遠停留在通道中。
    
        備註:正常情況下應該沒有必要修改該參數。
    
    
bridge priority (Bridge的相對優先級)

    優先級數字最低的橋將被選為root Bridge。root Bridge是生成樹"中心"的Bridge。
    
bridge forward delay

    設置轉發延遲時間。轉發延遲時間是在進入轉發狀態前，指的是每個Listening和Learning狀態的時間。
hello time

max message age

path cost

port priority(接孔優先等級)

stp(生成樹)



