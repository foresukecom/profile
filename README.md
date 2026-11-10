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

## スクリーンショット画像
「作ったもの」のスクリーンショットは `images/works/` に置く。  
1280x800 で撮影したものを 640x400 の WebP に変換する。

``` bash
magick screenshot.png -resize 640x400 -quality 85 images/works/xxx.webp
```

プロフィールアイコン (`images/はこね.png`) は 120x120
