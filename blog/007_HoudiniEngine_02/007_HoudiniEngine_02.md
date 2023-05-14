---
title: Houdini_007_HoudiniEngine_02
authors:
  name: いんと型
  title: 背景アーティスト・ディレクター
  url: https://github.com/wgao19
  image_url: https://github.com/wgao19.png
tags: [雑記]
---

# 007_HoudiniEngine_02


## 概要
- HoudiniとUEの連携をいろいろやってみる
- 今日は天球と床


## バージョン
UE4.27.2
Houdini19.5


## やり方
### その１
そもそもコリジョン
https://www.sidefx.com/docs/unreal/_collisions.html
とりあえずグループ作ってこれ入れておく
rendered_collision_geo
いけた
![](img/007_HoudiniEngine_02_2023-05-15-02-33-52.png)
サイズはともあれ、床完成

次は天球
面（プリミティブ）を反転するのはReverseで
![](img/007_HoudiniEngine_02_2023-05-15-02-52-41.png)
できた

Houdini上でのバックフェースカリングはここ
![](img/007_HoudiniEngine_02_2023-05-15-03-07-35.png)

テクスチャないけど一旦床と天球できた
![](img/007_HoudiniEngine_02_2023-05-15-03-20-02.png)

なんかuv作らないとクラッシュするっぽい
uv quickshade だとクラッシュするので、LabsAutoUV使ったらうまくいった

あとはnormalも直して適当に単色のマテリアルいれて今日はこんなもんで終了
![](img/007_HoudiniEngine_02_2023-05-15-03-55-43.png)

## おさらい
- コリジョンはグループに特定の名前つけると作れる　→　床
- UV作っておかないとすぐUEクラッシュする

## 次回予定
- カーブからなんか棒状のもの作る
- パラメータで太さとか変えられるようにする
- その際UVもある程度考慮して、トリムテクスチャとかあてる