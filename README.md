# profile

## セットアップ

開発環境は [Nix](https://nixos.org/) (flakes) と [direnv](https://direnv.net/) で構築します。  
画像のリサイズに使う ImageMagick などの開発ツールは `flake.nix` で定義しています。

### 前提

- Nix (flakes を有効化済み)
- direnv (シェルへのフック設定済み。[nix-direnv](https://github.com/nix-community/nix-direnv) の併用推奨)

### 手順

1. 本リポジトリを`git clone` する
1. リポジトリ直下で `direnv allow` を実行する (初回は開発ツールの取得に時間がかかります)

direnv を使わない場合は `nix develop` で同じ開発シェルに入れます。

## アイコン画像
以下コマンドで画像をリサイズ

``` bash
mogrify -resize 75x75 github.png
```

各種SNSのロゴは75*75  
フクロウアイコンは120*120
