#VTUN

VTUN是建立在TCP/IP網絡虛擬通道的最簡單方法。它支持各種通道類型，並提供了許多有用的功能：

    加密、壓縮、流量整形

VTUN很容易和高度可配置的。它可用於各種網絡任務： 

    VPN、Mobile IP、etc
    
通道型態

    IP 通道 (tun)
        支援點對點 IP 通道.
    Ethernet 通道 (ether)
        支援在以Ethernet上工作的所有協議: IP,IPX,Appletalk,Bridge,...
    Serial 通道 (tty)
        支援通過serial lines工作的所有協議：PPP，SLIP
    Pipe 通道(pipe)
        支持工作在UNIX pipes的所有程序。
        
通訊協定

    TCP:
        允許建立防火牆後面的通道。很可靠。
    UDP:
        快速高效的協議與小通道的。損耗