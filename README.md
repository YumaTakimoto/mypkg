# mypkg
[![test](https://github.com/YumaTakimoto/mypkg/actions/workflows/test.yml/badge.svg)](https://github.com/YumaTakimoto/mypkg/actions/workflows/test.yml)

このリポジトリは千葉工業大学先進工学部未来ロボティクス学科4sのロボットシステム学の講義で使用したものです。

# インストール方法
ROS2を使用できる環境でこのリポジトリをクローンして使用してください。

```
$ git clone https://github.com/YumaTakimoto/mypkg.git
```

# talker.py
* 数字をカウントし、/countupを通じてメッセージを送信するパブリッシャを持つノードです。
* 実行方法
```
$ ros2 run mypkg talker
```
* 実行結果
```
$ ros2 run mypkg talker
(なにも表示されないです。)
```

# listener.py
* /countupからメッセージをもらって表示するサブスクライバを持つノードです。
* 実行方法
```
$ ros2 run mypkg listener
```
* 実行結果
```
$ ros2 run mypkg listener
[INFO] [1703614615.311127831] [listener]: Listen: 35
[INFO] [1703614615.790040675] [listener]: Listen: 36
[INFO] [1703614616.289534774] [listener]: Listen: 37
[INFO] [1703614616.789775433] [listener]: Listen: 38
[INFO] [1703614617.290131362] [listener]: Listen: 39
[INFO] [1703614617.789669614] [listener]: Listen: 40
[INFO] [1703614618.290437826] [listener]: Listen: 41
[INFO] [1703614618.790250796] [listener]: Listen: 42
[INFO] [1703614619.290285793] [listener]: Listen: 43
[INFO] [1703614619.790167085] [listener]: Listen: 44
[INFO] [1703614620.290075553] [listener]: Listen: 45
[INFO] [1703614620.789807503] [listener]: Listen: 46
[INFO] [1703614621.290553867] [listener]: Listen: 47
(ctrl+cを押すまで表示し続けます。)
```

# talk_listen.launch.py
* talker.pyとlistener.pyを1つの端末で同時に立ち上げるノードです。
* 実行方法
```
$ ros2 launch mypkg talk_listen.launch.py
```
* 実行結果
```
$ ros2 launch mypkg talk_listen.launch.py
[INFO] [launch]: All log files can be found below /home/yumat/.ros/log/2023-12-27-03-52-54-605604-悠真のdynabook-2966
[INFO] [launch]: Default logging verbosity is set to INFO
[INFO] [talker-1]: process started with pid [2967]
[INFO] [listener-2]: process started with pid [2969]
[listener-2] [INFO] [1703616775.474445882] [listener]: Listen: 0
[listener-2] [INFO] [1703616775.952694410] [listener]: Listen: 1
[listener-2] [INFO] [1703616776.452376976] [listener]: Listen: 2
[listener-2] [INFO] [1703616776.952960683] [listener]: Listen: 3
[listener-2] [INFO] [1703616777.452338628] [listener]: Listen: 4
[listener-2] [INFO] [1703616777.952788539] [listener]: Listen: 5
[listener-2] [INFO] [1703616778.452249505] [listener]: Listen: 6
[listener-2] [INFO] [1703616778.952966532] [listener]: Listen: 7
[listener-2] [INFO] [1703616779.454496348] [listener]: Listen: 8
[listener-2] [INFO] [1703616779.953128713] [listener]: Listen: 9
(Ctrl+cを押すまで表示し続けます。)
```

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
