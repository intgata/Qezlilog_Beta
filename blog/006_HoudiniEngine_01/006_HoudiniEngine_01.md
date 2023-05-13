---
title: Houdini_006_HoudiniEngine_01
authors:
  name: いんと型
  title: 背景アーティスト・ディレクター
  url: https://github.com/wgao19
  image_url: https://github.com/wgao19.png
tags: [雑記]
---

# 006_HoudiniEngine_01


## 概要
- HoudiniとUEを連携、初めてやってみるときのログ
- とにかく簡単な.hdaを作ってUEに持っていく


## バージョン
UE4.27.2
Houdini19.5


## やり方
### その１
このサイトさんをみながらやってみる
https://papersloth.hatenablog.com/entry/2020/05/03/160408

昔やったときと違って、hda出力時の設定がいろいろあったので、そのうち内容を見ておく
命名規則的な


できた
パラメータどこかな？と思ったら、１つ下にちゃんと出ていた
![](img/006_HoudiniEngine_01_2023-05-14-02-49-12.png)

### その２
ここをみながら更にやってみる
https://support.borndigital.co.jp/hc/ja/articles/360001984014-Houdini-Digital-Asset%E3%82%92UnrealEngine%E3%81%A7%E4%BD%BF%E7%94%A8%E3%81%99%E3%82%8B

カーブをUE上で変更できるかと思ったけどできない・・

これを試してみる
https://www.youtube.com/watch?v=rN4Y6ucy_hY

カーブのバージョンを古いものに変えるみたい
![](img/006_HoudiniEngine_01_2023-05-14-03-31-39.png)
![](img/006_HoudiniEngine_01_2023-05-14-03-32-19.png)

できた！
![](img/006_HoudiniEngine_01_2023-05-14-03-37-13.png)

ノーマルがおかしいので、Normalノードとかはさむといいのかな？

Normalノードを足してから、hdaを更新する

更新のやり方は、以下の手順
1. Houdiniでアセットをセーブ
![](img/006_HoudiniEngine_01_2023-05-14-03-38-28.png)

1. UEで.hdaを右クリックからReImport
![](img/006_HoudiniEngine_01_2023-05-14-03-40-03.png)

1. rebuildを実行
![](img/006_HoudiniEngine_01_2023-05-14-03-40-38.png)


これでノーマルも入って見た目もある程度よくなった
![](img/006_HoudiniEngine_01_2023-05-14-03-41-20.png)

これでいろいろ実験できそう

## 次回予定
- UVいれて、テクスチャ・マテリアルを設定
- キャラが歩ける橋？とか作れるといいかも