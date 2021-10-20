# 中間発表テンプレート

明石高専の中間発表で使えるテンプレートです。Pugで書いてStylusで装飾した原稿をParcelでビルドして、vivliostyleでPDFにします。

# 導入

1. このリポジトリをcloneする
2. `$ yarn install` または `$ npm install`

# 執筆

文章を `src/index.pug` に書きます。デフォルトではPugを採用しています（ファイルを見ればわかりますが、シンプルに書けるHTMLです）。スタイルは `src/styles` にあります。特に書き換える必要はないでしょう。文中で使いたい画像は `src/assets/images` あたりに放り込んで、`src/index.pug`から相対パスで読み込めます。

# ビルド

`$ yarn build` または `$ npm build` でビルドできます。初回はレンダリングのためにChromiumをダウンロードするので時間がかかります（puppeteerをグローバルインストールしておくといいでしょう）。`resume.pdf` が出力です。

# ライセンス

スタイルは [yamasy1549/nitac_tex_template](https://github.com/yamasy1549/nitac_tex_template) を一部改変して使っています（`LICENSE` を参照）。それ以外の部分についてはパブリックドメインあるいはCC0とします。

# TODO

誰かやって

- 図のナンバリング
- Parcel V2
- https://github.com/sei0o/report-boilerplate と統合