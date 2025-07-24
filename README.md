# AutoLyricAnimation_K

![GitHub License](https://img.shields.io/github/license/korarei/AviUtl2_AutoLyricAnimation_K_Script)
![GitHub Last commit](https://img.shields.io/github/last-commit/korarei/AviUtl2_AutoLyricAnimation_K_Script)
![GitHub Downloads](https://img.shields.io/github/downloads/korarei/AviUtl2_AutoLyricAnimation_K_Script/total)
![GitHub Release](https://img.shields.io/github/v/release/korarei/AviUtl2_AutoLyricAnimation_K_Script)

AviUtl2でリリックモーションを行うためのスクリプト

[ダウンロードはこちらから．](https://github.com/korarei/AviUtl2_AutoLyricAnimation_K_Script/releases)

## 動作確認

- [AviUtl ExEdit2 beta1](https://spring-fragrance.mints.ne.jp/aviutl/)


## 導入・削除・更新

初期配置場所は`Transition (切り替え効果)`である．

### 導入

1.  同梱の`*.anm2`を`C:\\ProgramData\\aviutl2\\Script`フォルダまたはその子フォルダに入れる．

### 削除

1.  導入したものを削除する．

### 更新

1.  導入したものを上書きする．

## 使い方

- Ref Motion

  ここのトラックバーの移動を読み取り，リリックモーションを行う．この区間は1文字分であり，テキスト全体の長さではない．

  ここで設定できる移動方法であれば，どのような移動方法でもリリックモーションを行える．

  設定例: 0.0 -> 1.0 直線移動 (時間制御)

- Max Dist

  最大移動量．

- Spread

  開始，終了位置のランダムさ．

- Speed

  変化速度 (変化量倍率)．1倍のとき，1文字は100フレームで動作を完了する．

- Interval

  文字の登場間隔．変化速度によって間隔も変化する．

- Move X

  X軸方向に移動させる．

- Move Y

  Y軸方向に移動させる．

- Omni Dirs

  無効のとき右下から登場するが，有効にすることで上下左右からの移動を認める．

- Inv Dirs

  移動方向を反転させる．

- Type

  移動のタイプを指定する．

  - In: 登場

  - Out: 退出

  - In/Out: 登場と退出．退出時参照モーションは逆再生となる．

- Scale

  登場退場時の瞬間の拡大率．絶対値ではなく相対値である．

  `Entry`は登場時の瞬間拡大率，`Exit`は退場時の瞬間拡大率を意味する．%で指定．

- Rand Flip

  登場退場時に瞬間的に反転させる．反転確率は0.5．

  `Entry`は登場時のランダム反転，`Exit`は退場時のランダム反転の有効無効を意味する．

- Seed

  乱数発生のシード値を設定する．マイナスでレイヤーを移動させても値が変化しない．


## 謝辞

本スクリプトは，moll様が公開されている[全自動リリックモーション](https://drive.google.com/drive/folders/1DaBcNEEVqcmz6iUaLLFfUlsjwz39yyz3)を参考に作成いたしました．このような場をお借りして恐縮ではございますが，革新的かつ非常に有用なスクリプトを公開いただき，心より御礼申し上げます．

## License
LICENSEファイルに記載．


## Change Log
- **v1.0.1**
  - Spreadパラメータ0のとき移動しない問題の修正．

- **v1.0.0**
  - release
