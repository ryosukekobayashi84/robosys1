
#####myled.c  #ロボットシステム学　課題1
20c1044　小林凌介
##概要
入力する値（0,1）によってLEDが点灯、消灯するプログラムを上田先生のプログラムを元にＣ言語で実装しました。
##動画
-　https://youtu.be/HB9kV_G23-o
##使用するもの
  -Raspberry Pi 4
  -Ubuntu 18.04 LTS
  -LED
  -抵抗　300Ω

##使い方
1. リポジトリをクローンしてローカルリポジトリの作成
   $ git clone git@github.com:ryosukekobayashi84/robosys1.git
   $ cd robosys1
   
2.コンパイル、インストール
　$ make
  $ sudo insmod myled.ko
  $ sudo chmod 666 /dev/myled0 
3.実行
　$ echo 1 > /dev/myled0    //　点灯
  $ echo 0 > /dev/myled0　　//　消灯
4. 後始末
  $ sudo rm /dev/myled0
  $ sudo rmmod myled 
