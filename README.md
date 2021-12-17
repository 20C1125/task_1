# task_1
ロボットシステム学の課題１

授業動画を参考にLEDの追加とバッシュファイルで少しの遊びを入れた

# 使用したもの
ラズパイ３　B+   
ブレッドボード  
LED ジャンパー線  
抵抗　240Ω  

# 回路図  
![回路図](https://user-images.githubusercontent.com/95160686/146348393-3543b2cd-0b34-4897-8859-3f2edefb98ff.png)
# 使い方
$ make   
$ sudo rmmod myled    
$ sudo insmod myled.ko  
$ sudo chmod 666 /dev/myled0  
ここで準備完了  

 ・LEDを片方だけつける場合
 
LED 1 は $ echo 1 > /dev/myled0  
LED 2 は $ echo 3 > /dev/myled0    
消すとき  
LED 1 は $ echo 0 > /dev/myled0  
LED 2 は $ echo 2 > /dev/myled0      


 ・2つのLEDを使ったつく回数と切り替わる時間をコントロールするプログラム  
    
$ bash tempo.bash  
回数と切り替わりの時間を聞かれるので入力すると  
回数を表示しながら交互に光る  

# 動画
https://youtu.be/md04uxYqe_Q

# ライセンス  
GPL 3.0  
リンク↓　　

https://github.com/my9918/task_1/blob/master/COPYING　　
