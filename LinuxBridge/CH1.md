sudo apt-get install uml-utilities


新增虛擬網路介面卡

    $ sudo tunctl -b -u USER_NAME
    
    
新增一個橋接器
    
    $ sudo brctl addbr br0
    $ sudo brctl show
        
        bridge name     bridge id               STP enabled     interfaces
        br0             8000.000000000000       no
        
        
將橋接器接上實體網路卡

    $ sudo brctl adif br0 eth0
    $ sudo brctl show
    
        bridge name     bridge id               STP enabled     interfaces
        br0             8000.0cc47a715a90       no              eth0