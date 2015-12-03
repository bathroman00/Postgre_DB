#pgAdminまとめ

pgAdminとは
----------
pgAdminとはPostgreSQLを管理するツールである。  


使い方
-----
### 1.DBサーバ登録
アイコンをダブルクリック。  
![アイコン](http://www.fastpic.jp/images.php?file=7569151286.png "アイコン")

起動画面  
![起動画面](http://www.fastpic.jp/images.php?file=5007586116.png "起動画面")

起動画面でコンセントみたいな物をダブルクリック。  
![登録](http://www.fastpic.jp/images.php?file=6546857292.png "登録")

プロパティで名前、ホスト、Portを入力しOKボタンを右クリック。  
![登録](http://www.fastpic.jp/images.php?file=4061138219.png "登録")

### 2.DB接続
PostgreSQL9.4(localhost:5432)を右クリック。  
![登録](http://www.fastpic.jp/images.php?file=9333772043.png "登録")

パスワードを入力する。(設定によって自動で接続できる)  
![登録](http://www.fastpic.jp/images.php?file=6664332486.png "登録")

### 3.テーブル作成
「データベース」-「スキーマ」-「Public」-「テーブル」を右クリックし、  
メニュー内の「新しいテーブル」を選択する。  
![登録](http://www.fastpic.jp/images.php?file=4732774851.png "登録")

プロパティでテーブル名を設定する。  
プログラム言語を使ってDBのデータを取得する際に  
テーブル名が大文字だと認識できない場合があるため  
大文字は避けてほしい。  
![登録](http://www.fastpic.jp/images.php?file=7496168013.png "登録")

列を設定する。  
追加ボタンを右クリック。  
![登録](http://www.fastpic.jp/images.php?file=7790622982.png "登録")  

プロパティで名前、データ型を設定。  
![登録](http://www.fastpic.jp/images.php?file=5375794142.png "登録")  
列は後から変更することもできる。  

制約を設定する。  
追加ボタンを右クリック。  
![登録](http://www.fastpic.jp/images.php?file=0962368177.png "登録")  

プロパティで名前を設定する。  
![登録](http://www.fastpic.jp/images.php?file=3875140931.png "登録")  

列で主キーにしたい列を設定する。  
追加ボタンを右クリック。  
その後OKボタンを右クリック。  
![登録](http://www.fastpic.jp/images.php?file=5509140207.png "登録")  

外部キーを設定する  。
主キーを設定したときと同じ要領  
![登録](http://www.fastpic.jp/images.php?file=4503622477.png "登録")  
![登録](http://www.fastpic.jp/images.php?file=6632247614.png "登録")  
![登録](http://www.fastpic.jp/images.php?file=8938638365.png "登録")  

### 4.データ挿入
コマンドプロンプトでCSV形式の表をインポートすることができる。  
![登録](http://www.fastpic.jp/images.php?file=1404849950.png "登録")  

### SQL文 ###
	\copy テーブル名　from 'CSVがあるパス' with CSV;

試しにSELECT文で見てみると、  
![登録](http://www.fastpic.jp/images.php?file=1568379117.png "登録")  

データが入っていることがわかる。  


他にもいろんな機能があるが、  
触っていくうちに使い方がわかってくると思うので、頑張ってほしい。


ライセンス
----------
[PostgreSQL Licence][PostgreSQL]  
[pgAdmin Licence][pgAdmin]  

[PostgreSQL]: http://opensource.org/licenses/postgresql
[pgAdmin]: http://www.pgadmin.org/licence.php

