# mypkg
[![test](https://github.com/YumaTakimoto/mypkg/actions/workflows/test.yml/badge.svg)](https://github.com/YumaTakimoto/mypkg/actions/workflows/test.yml)

このリポジトリは千葉工業大学先進工学部未来ロボティクス学科4sのロボットシステム学の講義で使用したものである。

# インストール方法
ROS2を使用できる環境でこのリポジトリをクローンして使用する。  

```
$ git clone https://github.com/YumaTakimoto/mypkg.git
```

# talker.py
* 数字をカウントし、/countupを通じてメッセージを送信するパブリッシャを持つノードです

# listener.py
* /countupからメッセージをもらって表示するサブスクライバを持つノードです

# 必要なソフトウェア
* ROS2  
* Python
 
# テスト環境
* Ubuntu 22.04.2 LTS

# 著作権・ライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます． 
  * このパッケージのコードは，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．
  * [ryuichiueda/my_slides robosys_2022](https://github.com/ryuichiueda/my_slides/tree/master/robosys_2022)
* © 2023 Yuma Takimoto
