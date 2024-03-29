#  制限事項

| 制限項目                    | 制限内容                                                     | 補足                                       |
| :-------------------------- | :----------------------------------------------------------- | :----------------------------------------- |
| 外部接続通信                | Googleスプレッドシート<br />Googleドライブ<br />Slack(hooks.slack.com/slack.com) |                                            |
| ログ保存期間                | 6ヶ月                                                        |                                            |
| 1回の実行で出力できるログ量 | 100KB                                                        | 超えた場合、ログの出力は止まるが処理は継続 |
| 履歴保存件数                | 200件/6ヶ月                                                  |                                            |
| Script処理時間              | 10分                                                         |                                            |
| Script保存件数              | 1アカウント 100件                                            |                                   |
| Script容量                  | 5MB                                                          |                                            |
| URLリクエスト回数           | 10回                                                         | Script1回の実行あたりの上限                |
| URLリクエストサイズ        | 5MB                                                          |                                            |
| URLレスポンスサイズ        | 5MB                                                          |                                            |
| 動画/画像取扱いサイズ       | 20MB                                                         | 1ファイルあたりの上限<br />20MBのファイルを数回ダウンロードやアップロードするとエラーが発生する場合があります。<br />5MBサイズ程度の取り扱いを推奨します。|
| メール送信回数                 | 5回| Script1回の実行あたりの上限                | Script1回の実行あたりの上限                |
| メール送信容量                | 1MB                                                          |                                            |
| メールタイトル               | 10KB                                                          |                                            |
| メール送信先                  | <ul><li> Yahoo! JAPAN ビジネスIDに設定しているメールアドレスのみ </li><li> TO/CC/BCCそれぞれ10個まで</li></ul> | 広告アカウントに紐付いている参照/登録更新/管理者のいずれかの権限が付与されているYahoo! JAPAN ビジネスIDのみ送信可能|
| メール本文                      | 添付ファイル利用不可                                   |                                            |
| 天気取得可能日時                 | 当日、翌日                                           |                                            |
| 天気取得関数実行制限                 | 1回のスクリプトにつき20回まで                           |                                            |
