─── sample
    ├── app       ・・・アプリケーションのロジック
    ├── bootstrap ・・・laravelフレームワークの起動コード
    ├── config    ・・・設定ファイル
    ├── database  ・・・MigrationファイルなどDB関連
    ├── public    ・・・Webサーバのドキュメントルート
    ├── resources ・・・ビューや言語変換用ファイルなど
    ├── routes    ・・・ルーティング用ファイル
    ├── storage   ・・・フレームワークが使用するファイル
    ├── tests     ・・・テストコード
    └── vendor    ・・・Composerでインストールしたライブラリ


    php artisan serve --host=localhost --port=8000

#ルーティング定義の一覧を表示します。
    php artisan route:list

#マイグレーションファイルを作成
php artisan make:migration create_books_table --create=books
php artisan migrate
migrate:rollback
migrate:reset

#モデル作成
php artisan make:model Book

#コントローラーを作成
php artisan make:controller BookController