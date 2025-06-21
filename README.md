# CSV統合変換システム

Amazon・楽天・Yahoo のデータをヤマト運輸用CSVに変換するWebアプリケーションです。

## 機能

- マルチプラットフォーム対応: Amazon(TSV), 楽天(CSV), Yahoo(CSV)
- 商品マスタ連携: Excelファイルから重量・色情報を自動取得
- 住所統合: 同一配送先の注文を自動的にまとめて処理
- ヤマト運輸形式出力: 送り状システムに直接インポート可能

## デモ

公開URL: https://your-app.onrender.com


## 使用方法

1. 商品マスタファイル(Excel形式)を選択
2. ECサイトデータ(Amazon/楽天/Yahoo)を選択
3. 「データを変換してダウンロード」をクリック
4. ヤマト運輸用CSVをダウンロード


## ECサイトデータ
- Amazon: TSV形式(.txt/.tsv)
- 楽天: CSV形式(.csv)
- Yahoo: CSV形式(.csv)


## 技術仕様

- フロントエンド: HTML5, CSS3, JavaScript
- ライブラリ: PapaParse(CSV解析), SheetJS(Excel読み込み)
- 対応ブラウザ: Chrome, Firefox, Safari, Edge(最新版)


## ローカル実行

bashgit clone https://github.com/username/csv-converter.git
cd csv-converter
python -m http.server 8000

ブラウザで http://localhost:8000 にアクセス


## プロジェクト構成

```
csv-converter/
├── README.md
├── index.html
└── docs/manual.pdf
```

## 注意事項

- すべての処理はブラウザ内で完結（サーバーにデータは送信されません）
- 元データのバックアップを必ず取ってから変換を実行してください
