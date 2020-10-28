[English](README.en.md) | [日本語](README.md)

# jnmouse_description

[Jetson Nano Mouse](https://rt-net.jp/products/jetson_nano_mouse/)の[URDF](https://wiki.ros.org/urdf)等ハードウェア情報をまとめたROSパッケージです。

![](https://rt-net.github.io/images/jetson-nano-mouse/jnmouse_rviz.png)

## 動作環境

- ROS
  - [Melodic Morenia](http://wiki.ros.org/melodic/Installation/Ubuntu)

## インストール

```sh
# jnmouse_descriptionをダウンロードして依存パッケージをインストールします
cd ~/catkin_ws/src
git clone https://github.com/rt-net/jnmouse_description
rosdep install -r -y -i --from-paths .

# パッケージをビルドします
cd ~/catkin_ws
catkin build
source devel/setup.bash
```

## 使い方

Jetson Nano Mouseの[RobotModel](http://wiki.ros.org/rviz/DisplayTypes/RobotModel)をRViz上に表示するには以下のコマンドを実行します。

```sh
roslaunch jnmouse_description display_xacro.launch 
```

## ライセンス

(C) 2020 RT Corporation \<support@rt-net.jp\>

各ファイルはライセンスがファイル中に明記されている場合、そのライセンスに従います。特に明記されていない場合は、Apache License, Version 2.0に基づき公開されています。  
ライセンスの全文は[LICENSE](./LICENSE)または[https://www.apache.org/licenses/LICENSE-2.0](https://www.apache.org/licenses/LICENSE-2.0)から確認できます。

※このソフトウェアは基本的にオープンソースソフトウェアとして「AS IS」（現状有姿のまま）で提供しています。本ソフトウェアに関する無償サポートはありません。  
バグの修正や誤字脱字の修正に関するリクエストは常に受け付けていますが、それ以外の機能追加等のリクエストについては社内のガイドラインを優先します。


### 謝辞

https://gbiggs.github.io/rosjp_urdf_tutorial_text/index.html を参考にデータを作成しました。