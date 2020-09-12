# fk-bot-3
## 目的
FKを利用したトレードを完全自動化すること

## 利用する言語
Python: raspberry pi4 を制御する

## 処理の大まかな流れ
- タブレットの画面撮影
  - モータでカメラとリレータッチボードの座標を移動
  - リレータッチボードで画面タップ
  - カメラで撮影
- 画像処理
  - OCRを用いた画像認識 
  - 始値と（できれば）時刻の抽出
- FKルールと照合
  - FKのルールに則りFKステータスを更新する
  - サインを判定＆Slackに送信
- タブレットでの売買操作
  - リレータッチボードで証券アプリを起動
  - パスワードの入力
  - 売買の操作をタップして行う
    -「売り」「買い」の選択
    - 建玉の枚数
    - 成行きの選択んど
  
  