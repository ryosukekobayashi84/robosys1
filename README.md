
# ロボットシステム学　課題1
***20c1044　小林凌介***
## 概要 
入力する値（0,1）によってLEDが点灯、消灯する上田先生のプログラムをＣ言語で実装しました。
## 動画  
実際に動作している動画  
<https://youtu.be/HB9kV_G23-o>
## 使用するもの
  -Raspberry Pi 4  
  -PC   
  -LED  
  -抵抗　300Ω  
  -ブレッドボード  
  ## 環境  
  -Ubuntu 18.04 LTS 
  ## 使い方  
リポジトリをクローンしてローカルリポジトリの作成  
`$ git clone git@github.com:ryosukekobayashi84/robosys1.git`  
`$ cd robosys1`  
コンパイル、インストール  
 `$ make`  
 `$ sudo insmod myled.ko`  
 `$ sudo chmod 666 /dev/myled0`  
 実行  
 `$ echo 1 > /dev/myled0`    //　点灯    
 `$ echo 0 > /dev/myled0`　　//　消灯  
 後始末  
 `$ sudo rm /dev/myled0`  
 `$ sudo rmmod myled`  
 ## LICENCE  
 GNU General Public License v3.0  
 ## Author
 Ryuuichi Ueda 
 
 
 
