# 人間タワーバトル（2021年版）
動物タワーバトルの改良verをunityで動かすためのレポジトリ

このブログを参考にしました. http://blog.livedoor.jp/asamasou/archives/5689856.html

任意の写真(png)を追加すると落ちてきます．
土台から写真が落ちてしまったらゲームオーバーです．

<img src=https://github.com/murata-lab/unilab-tower-battle/blob/master/demo.JPG width=50%>

## 使い方
#### 1. unityをインストール
Unityをインストールする.

#### 2. レポジトリをクローン
```
git clone https://github.com/ak0592/unilab-tower-battle.git
```
をして，unityで開く．  
```
git clone https://github.com/ak0592/human_segmentation.git
```
をして，pythonの必要なリポジトリをインストールする。  
#### 3. タワーを作る
1. ProjectのAssets/Scenes/Mainを選択し，再生ボタンを押す.（画面の大きさは再生ボタン下のバーで変えられます.）
2. [segmentation](https://github.com/ak0592/human_segmentation)の使い方に従ってリアルタイムの画像処理を実行.
3. Assets/Resources以下にpng画像を追加され，写真が落ちてきてタワーに追加されます.
4. 再生ボタンを押すと終了します.

## 細かい仕様
- 高く積み上がったら画面からはみ出さないようにカメラが動いていきます.
- 再生ボタンが押された段階でAssets/Resources以下に画像があれば削除されます.
- unityが選択された状態でないと画像が落ちてこない場合があるので，その時は一回unityを選択してください.
