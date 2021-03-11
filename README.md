# macOSのデスクトップの壁紙を自動でセットアップするスクリプト

Mission Controlで複数のデスクトップを作ることができますが、このスクリプトは各デスクトップに壁紙を自動で設定してくれるものです。

Macを買い替えたりのタイミングなどでMacをセットアップするとき、壁紙の設定作業を楽にしてくれます。

## 使い方

### 必要なもの

実行にはHomebrewが必要です。インストールしておいてください。

### 必要な設定

1. Mission Controlでデスクトップを必要な数だけ作っておいてください。
1. キーボードショートカット設定で次を割り当てておいてください。
    - 「右の操作スペースに移動」: <kbd>^</kbd> <kbd>→</kbd>
    - 「デスクトップ1へ切り替え」: <kbd>^</kbd> <kbd>1</kbd>
    
### 壁紙画像を準備する

デスクトップの数と同じだけの枚数の画像を[images](./images)ディレクトリに用意します。

どのデスクトップにどの画像を配置するかは、01.jpg, 02.jpg, 03.jpg, ...のようにファイル名に順番をつけて表現してください。ファイル名の昇順で壁紙がセットされていきます。

対応している拡張子は.png, .jpg, .jpegです。

### 壁紙を設定する

[setup.sh](./setup.sh)を実行すると壁紙が順次設定されていきます。

```zsh
./setup.sh
```

## 動作確認したバージョン

macOS Catalinaでの動作確認はしています。

## Pro Tip

このリポジトリをDropboxなどのクラウドストレージにcloneしておくと、Macを買い替えたタイミングなどでスムーズに移行が行なえます。