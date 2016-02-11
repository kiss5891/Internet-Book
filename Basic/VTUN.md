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
        快速高效的協議與小損耗。
壓縮:

    Deflate (zlib):
        非常有效的壓縮，只支持HTTP
    LZO (lzo):
        超快的壓縮支援UDP、TCP

加密:

    基礎驗證:
        無明文密碼。
    BlowFish 128位密鑰:
        快速的高效的加密與128位元的MD5 Hash keys。

流量整理:

    可以限制通道內的進和出速度。
    
運行平台:
    
    Linux:
        RedHat, Debian, Corel
    FreeBSD and other BSD clones:
        FreeBSD 3.x, 4.x, OpenBSD, Apple OS/X 
    Solaris:
        Solaris 2.6, 7, 8, 9
    


參考文獻:http://vtun.info/features.html