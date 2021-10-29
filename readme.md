# コミュニティ向けのサイト構築

静的サイトジェネレータの MkDocs を活用して、Markdown記法でOSS版サイトのコンテンツを作成する。
公開は、GitHubと連携させて、静的サイトホスティングサービスにて公開する予定。


## コンテンツ制作者

### ローカル環境の準備

#### インストール

[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/getting-started/)

```
pip install mkdocs-material
```

[fontawesome_markdown](https://pypi.org/project/fontawesome-markdown/)

```
pip install fontawesome_markdown
```


#### ローカルでWebサーバ起動

```
# mkdocs.ymlファイルのあるフォルダへ移動

mkdocs serve -a localhost:5000
```

#### コンテンツの編集

Markdown(.md)ファイルを編集し、起動したサイトにアクセスして表示を確認する。


