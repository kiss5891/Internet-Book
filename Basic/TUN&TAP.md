#TUN與TAP

TUN與TAP是作業系統內核中的虛擬網路設備，在許多虛擬化網路技術都是基於這個介面來實現

什麼是TAP?
    
    

什麼是TUN?

    虛擬的點對點網路設備 TUN被設計為IP通道低水平核心支援
    提供了兩個給應用程式用戶使用的兩個接口
        - /dev/tunX	   - 裝置編號驅動
        - tunX	        - 虛擬點對點接口
    
    用戶應用程序可以寫IP frame到/dev/tunX 和內核將收到來自tunX 接口該frame。
    在同一時間的每frame內核寫入tunX接口可以通過用戶應用程序從/dev/tunX設備讀取。
    
支援的平台

    Linux kernels 2.2.x, 2.4.x 
    FreeBSD 3.x, 4.x, 5.x
    Solaris 2.6, 7.0, 8.0