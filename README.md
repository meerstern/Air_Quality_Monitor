# エアクオリティモニタ 
 Air Quality Monitor with ZMOD4410 & HS3001

  <img src="https://github.com/meerstern/Air_Quality_Monitor/blob/main/IMG/img1.jpg" width="360">
  ※ 写真は使用イメージです リップスティック、USBケーブル等は含まれません  

 ## 概要 
  *  [室内空気質（IAQ）センサZMOD4410][1]及び[温湿度センサHS3001][2]を搭載したエアクオリティモニタです 
  * スティック状の小型な本体にCO2値、IAQ(屋内空気質基準)、温度、湿度を表示することができます  
  * 電源はmicroUSBを介してUSB電源(5V/300mA)で駆動します  
  * CO2計算アルゴリズムはメーカ提供の学習済みニューラルネットワークを使用したファームウェアを使用しています  
  * 学習済みニューラルネットワークによって従来よりもより正確にCO2値（eCO2）を推定できます  
  * 専用変換基板のLEDでIAQ(屋内空気質基準IAQ:2以下 青、2-3:青、黄、3-4:黄、4-5:黄、赤、5以上:赤)を確認できます 
  * 過去10時間の推移をグラフで簡易的に確認することができます  
  * 寝室等での利用を想定し、周辺の明るさに応じてLED及びOLEDの輝度が低下する機能を搭載しています  
  * ボタン切り替えでCO2表示モード、温度表示モード、湿度表示モード、IAQ表示モードの切り替えが可能です  

   
  |  項目  |  範囲  | 
| ---- | ---- | 
|  温度  |  -40-125℃  |   
|  湿度  |  0-100%RH  | 
|  CO2  |  400-5000ppm  |  
|  IAQ  |  1.0-5.0  |  
    
 ドイツ環境庁（UBA）の屋内空気質（IAQ）基準
 
  |  IAQ  |  レベル  |  LED  |
| ---- | ---- | ---- |
|  <2  |  非常に良い  |  青  |
|  2~3  |  良い  |  青と黄  |
|  3~4  |  中間  |  黄  |
|  4~5  |  悪い  |  黄と赤  |
|  5~  |  非常に悪い | 赤 |
    
  <img src="https://github.com/meerstern/Air_Quality_Monitor/blob/main/IMG/img2.jpg" width="360"> 

  <img src="https://github.com/meerstern/Air_Quality_Monitor/blob/main/IMG/img3.jpg" width="360"> 

## 注意 
 * 本センサはMOX(Metal Oxide)式のCO2センサのため、空気中の有機物から間接的にCO2に換算します  
 * 厳密なCO2計測には向きません  
 * 安定した測定をするために人通りや気流の変化が少ない場所に設置して使用してください  
 * キャリブレーション後にCO2値が安定するまで約0.5~1時間程度要します  
 * IAQは総合的な空気質の指標のため、CO2値が低くても他の有機物が多い場合に高くなります  
 * 電源投入後、2~3分はキャリブレーションのため、温湿度以外の値は未定で、全LEDが点灯します  
 * 約2秒周期で各センサの値を取得します(データ更新時にLEDが点滅します)  
 * センサのデータ応答が異常な場合、自動的に再起動する場合があります  
 * 再起動した場合はグラフの履歴がリセットされます  
 * 告知なしに仕様を変更する場合があります   
 * 背面のセンサ穴を塞がないように設置してください   

  <img src="https://github.com/meerstern/Air_Quality_Monitor/blob/main/IMG/img4.jpg" width="360"> 
  
[1]: https://www.idt.com/jp/ja/products/sensor-products/gas-sensors/zmod4410-indoor-air-quality-sensor-platform
[2]: https://www.idt.com/us/ja/products/sensor-products/humidity-sensors/hs3001-high-performance-relative-humidity-and-temperature-sensor

