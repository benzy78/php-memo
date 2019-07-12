# php学習メモ

## foreach文
配列の内容をループ処理で取り出す処理

## PHPの終了タグの扱いについて
PHPの終了タグ **?>** は省略可能。
終了タグの後に不要な余白などがあると、予期せぬエラーや表示のズレが生じることがあるので、基本的にHTMLが存在しない、PHPだけの場合は終了タグは省略することが推奨されている。

## action属性とmethod属性
`<form action="output.php" method="post">`
action属性は入力されたデータの送信先をスクリプトで指定し、サーバ側でデータを受け取るプログラムを指定して使う。

method属性はフォームの内容をサーバーに送信するために使用するもの。基本的にはPOSTを使う。

## GETとPOSTの違い
GETはデータの取得に使われることが多いが、POSTと同じようにデータの送信にも使える。
GETは、URLの後ろに送信したいデータを付与してデータを送信するのに対して、POSTはHTTPリクエスト内のメッセージボディに送信したいデータを入れて送信する。
GETだと、URLの後ろに送信したいデータを付与するため、ブラウザの閲覧履歴にデータの送信内容が残ってしまうため、ユーザーのIDやPassWord、お問い合わせFormの内容などはPOSTを使う必要がある。

## プログラミングの勉強
重要だなと思ったところはマーカー引いて、その後何も見ずにこのGithubにまとめる。（Daigo式）
また、一章や区切りのいいところで、本を閉じて内容を自分の言葉で説明してみる。

## PHPの変数のルール
1. 変数名の前にはドル記号（　$　）をつける。
2. 一文字目には英字もしくは、アンダースコア（　_　）を使う。
3. 二文字目以降は英字、数字、アンダースコアのいずれかを使う。
4. 英字の大文字と小文字は区別される。

## isset関数
isset関数は、変数に値が代入されていて、かつ値がNULL出ないときに、TRUEを返す関数。

より、簡単にいうと、変数が定義されているかどうかを調べる関数。

## 返り値（戻り値）
関数の実行が終了すると、関数の呼び出し元に、処理の結果の値を返す。この値を返り値もしくは戻り値という。

## データベースについて
データベースを構築・操作するソフトフェアをデータベース管理システムという（DBMS）。

近年よく利用されるデータベースは、関係データベースと呼ばれるもので、その関係データベースの管理システムを関係データベース管理システム（RDBMS）という。

そのRDBMSの中にMariaDB、MySQLなどがある。ちなみにMariaDBはMySQLの派製品。

で、RDBMSを利用するために使うのが、SQLというプログラミング言語。

データベースの基本操作は、生成、読み取り、更新、削除この４つ。それぞれの頭文字をとって、CRUDとも言う。

## セッションについて
セッションとは、Webアプリケーションにおいて、各ユーザーの固有のデータを管理するための仕組み。
これによって、ログイン機能や、ショッピングサイトのカートの機能を実装できる。

## これをおえてのアウトプット
コンセプトは役に立つもの。ただのポートフォリオにはしたくないんだよな。

機能としては
1. ログイン機能
2. お気に入り機能
3. 投稿、更新機能
