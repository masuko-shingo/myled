# myled
robosys2019 課題

# 動作環境
ubuntu16.04
Rasberry pi Model 3B+

実行方法
$ git clone 
$ cd myled
$ make
$ sudo insmod myled.ko
$ sudo chmod 666 /dev/myled0
$ sudo echo 1 > /dev/myled0
$ sudo echo 2 > /dev/myled0
$ sudo echo 0 > /dev/myled0
$ sudo rmmod myled.ko
