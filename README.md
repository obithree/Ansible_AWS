AWS上にphpMyAdmin実行環境構築プレイブック
更新日：20180827
作成者：obithree

ただコピーしただけでは起動しません。
ディレクトリに配置後、変数を設定する必要があります。

例
・phpmyadminの設定ファイルのテンプレートのパス
phpmyadmin1_src: /home/ec2-user/ansible/pMA_AWS/roles/3.apache/files/phpMyAdmin.conf
phpmyadmin2_src: /home/ec2-user/ansible/pMA_AWS/roles/3.apache/files/config.inc.php

また、playbookを実行するサーバにIAMロールといった権限が必要です。
CentOS上でやる場合、AWSCLIをインストールし、aws configureで権限を与える必要があります。

細かな実行環境はは後日記入します。
playbookの解説も後日コメントアウトで入れえる予定です。
