# train-alarm

作品名：TrainAlarm<br>
作成期間：2020年11月～2021年２月<br>
言語：PHP<br>
DB：MySQL（MariaDB)<br>
フレームワーク：jQuery、Bootstrap<br>
開発環境：PHPStorm

概念：<br>
このプロジェクトは、公共交通機関のAPIを利用して構築されたもので、トレインアラーム設定システム。
<br>

使い方：<br>
設定画面では、4つの入力がユーザーに求められます。その後、メインスクリプトは、入力された情報に基づいて、APIを処理し、エラーが発生しなければアラームが設定され、設定が完了しました。

機能：<br>
登録されたユーザーは、自分の利用履歴にアクセスし、お気に入りを選択することができます。また、ログイン時には、ユーザーがアクティブなアラームを持っているかどうかをチェックし、持っている場合はアラーム画面にリダイレクトします。
<br>
登録したくないユーザーもこのアプリケーションを利用できます。その際、アラーム設定情報と一緒に電話番号の入力が必要となります。その後、アラーム画面に戻るには、トップメニューから「アラーム確認」を選択し、使用した電話番号を入力します。

ファイル概念：<br>

/access<br>
dbh.access.php・・・データベースへの接続

/add<br>
footer.add.html・・・各ページのフッター<br>
header.add.php・・・各ページのヘッダー<br>
error_handler.add.php・・・各ページでエラーと成功のビジュアルフィードバックを処理
<br>

/function<br>
functions.js ・・・index.phpファイルのアラーム設定フォームで使用されます。<br>
functions.php・・・includesディレクトリにあるファイルで利用されますファンクション。

/includes<br>
ここにあるファイルは、メインディレクトリ上のそれぞれのファイルへの入力検証とデータベースアクセスを処理します。
alarm.inc.php・・・このアプリケーションAPI処理スクリプトを含む<br>

/ メインディレクトリ<br>
ここにあるファイルは、ウェブページを構築するためのレイアウトを持っています。