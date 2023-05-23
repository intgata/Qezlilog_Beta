---
title: UE4_003_HoudiniEngineスターターキット_01
authors:
  name: いんと型
  title: 背景アーティスト・ディレクター
  url: https://github.com/wgao19
  image_url: https://github.com/wgao19.png
tags: [雑記]
---

# 003_UE4_HoudiniEngineStarterKit_01


## 概要
HoudiniとUEを連携、初めてやってみるときのログ



## バージョン
UE4.27.2?


## やり方
ここへアクセス
https://www.sidefx.com/ja/tutorials/ue4-starter-kit/

キットをダウンロード
自分の環境のフォルダパスたくさんありますので参考程度に

キットの場所
E:\Learn\Houdini\EngineUE4\GameJamStarterKit-UnrealEngine5\GameJamStarterKit-UnrealEngine5

次に、UE4とHoudiniの連携をセッティング
この動画をみつつ

Houdiniフォルダ側
C:\Program Files\Side Effects Software\Houdini Engine\Unreal\19.5.493\4.27\HoudiniEngine

UE4フォルダ側
E:\Program Files\Epic Games\UE_4.27\Engine\Plugins\Runtime

UEプロジェクトはここ
E:\Learn\Houdini\EngineUE4\TEST_GameJam

プロジェクト
ブランクで作成したもの
まずプラグインを確認
![](img/003_UE4_HoudiniEngineStarterKit_01_2023-05-13-03-47-51.png)
チェック入っているのでよさそう

よくみるとメニュー的なところにHoudiniEngineが入っている
![](img/003_UE4_HoudiniEngineStarterKit_01_2023-05-13-03-48-34.png)

hdaをドラッグアンドドロップで動作した！
![](img/003_UE4_HoudiniEngineStarterKit_01_2023-05-13-03-52-16.png)
（一瞬計算みたいなのがはしった）

とりあえず動いて、パイプだったらカーブとかいじると変形するのが確認できた

## 次回やること
ただ、、パラメータが多いので、どこが.hdaに起因するものかとか、メッシュのベイク？とか
共通のパラメータとか知るために、いったん簡単な.hdaを作ってみてどうなるか　次回やってみる


## そのほか
ここにもいろいろ動画ある
https://vimeo.com/442124384
フォリッジツールとか面白そう