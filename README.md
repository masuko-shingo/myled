# myled
robosys2019 課題

### 動作環境
|||
|:--:|:--:|
| Raspberry Pi | Raspberry Pi Model 3B+ |
| OS | Ubuntu18.04 |

### 実行方法
```
$ git clone 
$ cd myled
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
$ sudo echo 1 > /dev/myled0
$ sudo echo 2 > /dev/myled0
$ sudo echo 0 > /dev/myled0
$ sudo rmmod myled.ko
```
echo 1で緑色のLED,echo 2で赤色のLED,echo 0でLEDを消灯させる．

### Demo
https://www.youtube.com/watch?v=1L0XntVSnkU
