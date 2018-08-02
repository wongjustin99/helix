# Helix Beta Build Guide (Google Translated)


## Parts

Below is the number of parts needed to make one. Two sets are necessary to make two hands.

| Name | Number | Remarks |
| ---- | ---- | --- |
| PCB | 1 sheet | |
| Pro Micro | 1 | |
| TRRS jack | 1 | |
| Tactile switch | 1 | |
| スプリングピンヘッダ 12P | 2個 | 通常のピンヘッダでも可 |
| プレート（アクリルかステンレス） | 1セット| |
| 保護プレート | 1枚 | |
| M2スペーサー 4mm | 6個 | ロープロファイルスイッチ用 |
| M2スペーサー 7mm | 6個 | MX互換スイッチ用 |
| M2スペーサー 8mm | 2個 | |
| M2ネジ 3mm| 14個 | |
| M2低頭ネジ 5mm| 2個 | |
| ゴム足 | 6個 |  |
| ダイオード | 32個 | ロープロファイルスイッチを使用する場合はSMDのダイオードが必要です。 |
| キースイッチ | 32個 | KalihロープロファイルあるいはMX互換 |
| キーキャップ | 32個 | キースイッチと互換があるもの |
| 3.5mmオーディオケーブル | 左右合わせて1本 | 左右のキーボード接続用 |
| micro USBケーブル | 左右あわせて1本 | |
| 絶縁シート | 1枚 | ステンレスプレート用（オプション）|
| LEDストリップ（WS2812B 6個付き） | 1個 | Underglow用（オプション） |
| SK6812mini | 32個 | バックライト用（オプション） |
| OLEDモジュール | 1個 | OLED用（オプション） |
| ピンソケット 4P | 1個 | OLED用（オプション） |
| ピンヘッダ 4P | 1個 | OLED用（オプション） |

## 必要な道具

| 名前 | 備考 |
| ---- | ---- |
| はんだごて | バックライトLEDを使用する場合は調温出来るもの |
| 糸ハンダ | 0.8mm程度のものを推奨 |
| ピンセット | チップ部品実装時 |

## 構成の選択
制作を始める前にどのような構成にするか決めておく必要があります。

### 行数の選択（５行または４行）
PCBを切断することによってデフォルトの５行から４行へ変更することができます。


### LEDの選択（Underglowかバックライト）
テープLEDを使用したUnderglowか、チップLEDを使用するバックライトを選択します。

## 組み立て方

以降は左手用で説明します。右手用はPCBを反転して下さい。

![Imgur](https://i.imgur.com/N4rZw99.jpg)

__一度全ての工程を読み、理解してから作業を進めることをお勧めします。__

### PCBの準備

オプションのOLEDモジュールを使用するときはPCBにジャンパが必要になります。
左右ともに**上面側**の４箇所をジャンパします。
（両面をジャンパしてはいけません）

![Imgur](https://i.imgur.com/nKrfKwf.jpg?2)



### パーツ実装

#### ダイオード

リードタイプ、チップタイプ共にPCBの**下面側**から実装します。

ダイオードには向きがあるので注意してください。
シルクが見えなくなっているところがありますが、全て同じ方向なので他に合わせてください。


![Imgur](https://i.imgur.com/HNnsSsT.jpg?2)

![Imgur](https://i.imgur.com/nSBrYvQ.jpg?1)

#### バックライトLED（オプション）

バックライト用のチップLEDはPCBの**下面側**から実装します。向きに注意して穴に入れてください。裏から見て、一番大きいパッドとシルクの○が同じ位置になります。


シルクが見えなくなっているところがありますが、同じ行は同じ向きですので見えるところを参考にしてください。また、行ごとに向きが変わるので注意してください。

調温半田ごてを使い、約220℃ではんだ付けします。__温度が高いとLEDが壊れますのでご注意ください__。

![Imgur](https://i.imgur.com/omUY0ac.jpg?2)

![Imgur](https://i.imgur.com/Sdb0xIW.jpg?2)



1行分まとめてLEDを並べて一番大きいパッドだけ仮で半田付けしてから、残りの部分をはんだ付けすると、効率よくつけられます。




#### TRRSジャック

シルクにしたがって上面から実装してください。

![Imgur](https://i.imgur.com/C5P0kDs.jpg?2)


#### リセットスイッチ

タクトスイッチを上面から実装してください。

![Imgur](https://i.imgur.com/K2FCjWh.jpg?2)

#### Pro Micro

スプリングピンヘッダをPro Microに半田付けします。Pro Microの裏面（平らな方）が上になるようにします。

![Imgur](https://i.imgur.com/pasAMct.jpg)

スプリングピンヘッダには推奨する向きがあります。

![Imgur](https://i.imgur.com/GyAEU3l.jpg)

小さい窓がPro Micro寄りになります。
また、実装時には二本ともに小さい窓が同じ方向を向くようにしてください。

![Imgur](https://i.imgur.com/QsmOP1X.jpg)

![Imgur](https://i.imgur.com/nvFQElc.jpg)

※向きを間違えたり、はんだ付けする前に強い力がかかるとピンが外れますので注意してください。また、足が折れ曲りやすいので抜き差しするときには注意して扱ってください。

裏面を上にしてPCBの白枠線内のスルーホールに取り付けてください。はんだ付けしなくても固定されます。

![Imgur](https://i.imgur.com/Hj5YHhp.jpg)


#### OLEDモジュール（オプション）

ピンソケットを上面に実装し、ピンヘッダをOLEDモジュールに半田付けします。
そしてPro Microの上に被せるようにしてピンソケットに差し込みます。


![Imgur](https://i.imgur.com/Uy9osXH.jpg)

![Imgur](https://i.imgur.com/9K3uwFV.jpg)


#### Underglow用テープLED（オプション）

向きに注意して裏面に直接実装するか配線材を使って実装してください。

![Imgur](https://i.imgur.com/hkJUmcZ.jpg)

#### キースイッチ

マウントプレートを挟んでPCBに実装します。
狭いところは隣のパッドにブリッジしないよう気をつけて下さい。

![Imgur](https://i.imgur.com/w8b6SMt.jpg)

※ここまで来たら一旦[ファームウェア](firmware_jp.md)を書き込み、動作確認をした方が良いでしょう。


### 最終組み立て

8mmのスペーサーを2本、PCB上面にネジ止めします。

![Imgur](https://i.imgur.com/pNzGs7G.jpg)

ロープロスイッチは4mm、MXキースイッチは7mmのスペーサーを使い、PCBをサンドイッチするように底面用のプレートをネジ止めします。

![Imgur](https://i.imgur.com/FWfX1rQ.jpg)

保護プレートを8mmのスペーサーに低頭ネジを使ってネジ止めします。

![Imgur](https://i.imgur.com/YsHOSRJ.jpg)

ゴム足を底面に貼ります。

![Imgur](https://i.imgur.com/b6dDQVc.jpg)

完成です。

![Imgur](https://i.imgur.com/WEFh37i.jpg)
