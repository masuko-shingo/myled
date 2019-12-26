# myled
robosys2019 課題

### 概要
LED(赤×１，緑×１)と抵抗×２を使い入力によって光るLEDの色を変えるプログラムです．

### 動作環境
|||
|:--:|:--:|
| Raspberry Pi | Raspberry Pi Model 3B+ |
| OS | Ubuntu18.04 |

### 実行方法
```
$ git clone https://github.com/todasayaka/myled.git
$ cd myled
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
$ sudo echo 1 > /dev/myled0
$ sudo echo 2 > /dev/myled0
$ sudo echo 0 > /dev/myled0
$ sudo echo 2 > /dev/myled0
$ sudo echo 1 > /dev/myled0
$ sudo echo 0 > /dev/myled0
$ sudo rmmod myled.ko
```
echo 1で緑色のLED,echo 2で赤色のLED,echo 0でLEDを消灯させる．

### 回路図
![kairo](https://user-images.githubusercontent.com/58972091/71457728-b28e8c00-27e2-11ea-8970-7b9088bc6939.PNG)

### Demo
https://www.youtube.com/watch?v=1L0XntVSnkU
