---
title: 002_Houdini_出力まわり
authors:
  name: いんと型
  title: 背景アーティスト・ディレクター
  url: https://github.com/wgao19
  image_url: https://github.com/wgao19.png
tags: [雑記]
---

# まずはキューブ作る
- ただのキューブだとわかりにくいので２個つなげる
![](img/002_Houdini_Export_2023-04-30-01-36-31.png)

## 書き出しとインポート
- fbx書き出し
File ▸ Export ▸ Filmbox FBX を選択します。
（Filmboxっていうんだ・・）

出力先を入力すると、exportができるようになります

UE4にインポートするとやたら小さいのでスケール１００倍したらそれっぽくなりました
![](img/002_Houdini_Export_2023-04-30-01-57-00.png)
Houdiniは単位がメートルで、UEはセンチなんだとか
インポート設定は特にいじっていない

## マテリアルのアサイン
フェースアサインでマテリアルを入れてみる
同じフェースを指定するとあとで指定したほうのマテリアルが出力される（そりゃあそうだ）
![](img/002_Houdini_Export_2023-04-30-02-27-12.png)
