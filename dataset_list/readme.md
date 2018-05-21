# データセット一覧を作成するためのエクセルツール
## 使い方
エクセルファイルを開いてクエリを更新してください。

![説明1](https://raw.githubusercontent.com/City-of-Kobe/opendata_dashboard/master/dataset_list/img/datasetlist_inst1.png)


## 解説
### 概要
神戸市オープンデータポータルに掲載されているデータセットのメタ情報をCKAN APIを通じて取得し、エクセルのテーブルに変換するツールです。
CKAN APIではjson形式で提供されるため、それをエクセルのクエリ機能（PowerQuery）を利用して変換します。
※以下の内容はMicrosoft Office 2013 + Powerqueryで行っています。それ以外の環境では画面が一部異なることがあります。

### EXCELクエリの作成方法
1. Excelを開き、POWER QUERY -> WEBから　を選択
1. 「<https://data.city.kobe.lg.jp/data/api/action/current_package_list_with_resources?limit=200>」と入力しOKをクリック
1. クエリエディタが開くので、resultの行の「List」の文字列がリンクになっているのでクリックする。
![説明2](https://raw.githubusercontent.com/City-of-Kobe/opendata_dashboard/master/dataset_list/img/datasetlist_inst2.png)
1. 列のタイトル（「一覧」と表示されているところ）を右クリックして、テーブルに変換をクリック。次に表示されるテーブルへの変換のダイアログのそのままOKをクリック。
![説明3](https://raw.githubusercontent.com/City-of-Kobe/opendata_dashboard/master/dataset_list/img/datasetlist_inst3.png)
1. Column1を展開
![説明4](https://raw.githubusercontent.com/City-of-Kobe/opendata_dashboard/master/dataset_list/img/datasetlist_inst4.png)
1. 項目を整理
groupsやorganizationなどの項目も同様に展開。不要な項目の削除や並べ替えを行う。適宜、項目名称の変更を行う。
