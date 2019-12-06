### TODO

- セル機能を導入せべし、矢印でセルを移動、Enterでセルの編集を行う
- ポップアップ機能でユーザに通知を行うこと => react-pnotify導入予定
- DeleteDimensionComponentを作成すること
- タイトルコピーボタン欲しい
- データの削除機能ほしい
- データを読み込むときに空の改行を読みとばす処理を入れたい
- eslint、jest導入したい => eslintめんどくさい、jestは入れる
- 出力時に存在確認したい

### 暫定対処

- ファイルを分割する

```sh
$ split -d -l 100 --additional-suffix=.csv prod.csv prod-split
$ ls prod-split* | xargs sed -i '1s/^/title\n/'
```