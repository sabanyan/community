--8<-- "includes/glossary.md"

# 行ずらし : mslide

項目の値を指定した行数ずらして出力します。<br>

表形式のデータに対して、特定の項目だけ、値の位置を指定の方向と行数だけずらしたい場合に使用します。
グループを指定すると、異なるグループにまたがった値のずらしを回避できます。


## <i class="fa fa-arrow-circle-right" aria-hidden="true"></i> 活用シーン



## <i class="fa fa-arrow-circle-right" aria-hidden="true"></i> 使用例



## <i class="fa fa-arrow-circle-right" aria-hidden="true"></i> コマンドの選択


## <i class="fa fa-arrow-circle-right" aria-hidden="true"></i> オプションの設定

??? Abstract "グループの設定（必須）"
    ■グループ化する項目名　(省略可)
    :  引数名 = k <br>
    
         - 項目名を指定すると、その値が同じグループごとに処理
         - カンマ区切りで複数指定可
         - 省略時は全ての行を同じグループとみなして処理される
    
    ■グループ内ソートの設定 (必須)
    :  引数名 = s <br>
        
         - ソートのキー項目を、カンマ区切りで複数指定可
         - 方法: 項目名末尾に記号を付与<br>
            (数値昇順：%n,  文字列降順： %r,  数値降順：%nr)
        !!! warning "注意"
            グループ化する項目名と同じ項目名があると、不整合になり、ソートされません

??? Abstract "行ずらしの設定 (必須)"
    - 指定した行数先までの全ての値を、当行に持ってくる
    - 追加列名は 元の列名と行数を組合せで自動生成される
    
    ■対象とする項目名 (必須)
    :   引数名 = f

         - カンマ区切りで複数指定可
         - ワイルドカード(*,？ )使用可

    ■ずらし行数の指定 (必須)
    :   引数名 = t

         - 1以上の整数で指定する 
         - [ ] 先の行ではなく、前の行から持ってくる
         - [ ] 持ってくる先がない場合には、行削除ではなく、値をNullとする
         - [ ] 指定した行数全てでなく、最後の行のみ持ってくる

??? Abstract "その他 (省略可)"
    - [ ] 自動並べ替えの無効化
    - [ ] 入力データの1行目を項目名行とみなさない
    - [ ] 出力データに項目名行を出力しない
    - [ ] 項目名ではなく、項目番号で指定する

??? Abstract "システム管理用設定（作業領域・ログ出力）"
    - 作業ファイル格納パス名
    - [ ] 入力、出力件数比較を行う
    - [ ] 出力項目のNULL値チェックを行う
    - [ ] キー項目にNULL値が含まれているかどうかのチェックを行う
    - [ ] 対象とする項目名で指定された項目のNULL値チェックを行う



## <i class="fa fa-arrow-circle-right" aria-hidden="true"></i> 関連情報


!!! info
    処理は[nysol mcmd](https://www.nysol.jp/nysol_python/mcmd/methods/mslide.html)で行います。

<!-- [nysol mcmd](https://www.nysol.jp/nysol_python/mcmd/methods/mslide.html) -->


