# nccu_drone

## Space Model

Space Model contains two fields：

* DroneContext
* MapContext

#### DroneContext
###### Attribute
* currentPoint - 表示現在位置，return Point(x,y,z)
* blockList - 障礙物 list
* path - 經過的路徑，每次移動呼叫 move()時，會把現有位置持續保存形成路徑
###### Function
* move(x,y,z) - 無人機移動時呼叫

#### MapContext
###### Attribute
* roomAge - 整個空間的大小，使用 setRoomAge 後把值存在這
* heightSpace - 某一高度有的建築或物體

###### Function
* add_space(height,[][])
* set_room_age(length,width,height) - 設定整個空間初始的長寬高

## Q & A
* 無人機移動的流程，呼叫順序
* 空間的設置，x y z 的初始位置，四個角或中間
