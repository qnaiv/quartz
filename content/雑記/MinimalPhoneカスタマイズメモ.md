---
publish: true
created: 2026-07-28T00:02:53.429+09:00
modified: 2026-07-29T23:47:26.802+09:00
---

# 日本語入力

- [[aquamozc]] [[minimalphone]]版を導入
   - 絵文字キー、SYMキーの動作をカーソル移動に変更
  - ​ショートカット
    　 - Alt+Space=変換
    　 - 左Shift=Ctrl
    　 - Micキー=ハイフン
  - 文字入力時
    　   - Ctrl+UIOP=ひらがなカタカナ半角全角切り替え
- ホームランチャーをniagara launcherに変更
  - ホーム画面で文字キーを押すことでアプリを絞り込めるようになる

# Key mapper

物理キーボードを有効活用するためにkeymapperを導入して文字キーに対して色々なショートカットを割り当てた。設定が多少面倒だが、画面を触る頻度が圧倒的に減って良い。
お気に入りはB、Vキー長押しで輝度変更してバックライトをオン・オフできるのと、Kindleを読むときにH、Kキーでページ送りができるところ。（ボリュームキーでもページ送りできるが、持ちなおすのがちと面倒。）

## 設定のポイント

ポイントはTriggerを長押しでDo not remapにすること。これで短押しの場合は文字入力になり、長押しの場合のみ動作するようにできる。（テキストボックスにフォーカスしている状態だと文字が打たれ続けてしまうが…）

## 注意点

- ==Xはデフォルトで文字キーにショートカットが指定されており、例えばUキーを押すとミュートが発動してしまうため、誤爆に注意。==
- 何故かたまにアクションが無限実行されてしまうことがあるが、そんなときは再度キーを長押しすれば解除される。

## 設定したもの

- ​J長押し: 下にスクロール
  - Trigger
    - JキーLongPress, Do not remap
  - Action: Swipe Screen
    - StartX0→EndX0
    - StartY400→EndY300
    - SwipeDuration50
- ​U長押し: 上にスクロール
  - Trigger
    - UキーLongPress, Do not remap
  - Action: Swipe Screen
    - StartX0→EndX0
    - StartY300→EndY400
    - SwipeDuration50
- ​H長押し: 左にスクロール
  - Trigger
    - HキーLongPress, Do not rem
  - Action: Swipe Screen
    - StartX200→EndX400
    - StartY100→EndY100
    - SwipeDuration200
- ​K長押し: 右にスクロール
  - Trigger
    - KキーLongPress, Do not rem
  - Action: Swipe Screen
    - StartX400→EndX200
    - StartY100→EndY100
    - SwipeDuration200
- N長押し: 通知を開く
- B長押し: 画面輝度を上げる
- V長押し: 画面輝度を下げる
- E長押し: Edge起動
- X長押し: X起動
