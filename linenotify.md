**俺モニター**からの通知をLINEで受信するための手順を説明します

目次

1. [はじめに](#introduction)
1. [Google Cloudコンソールでの手順](#googlecloudconsole)
1. [Googleスプレッドシートでの手順](#googlespreadsheet)
1. [俺モニターでの手順](#oremonitor)

---

<a id="introduction"></a>

# はじめに
**俺モニター**からの通知をLINEで受信できるようにするために、**LINE Notify**を利用します。

大まかな手順の説明です。

1. LINE Notifyアカウントを自身のLINE友達に加える
1. アクセストークンを発行する
1. **俺モニター**にアクセストークンを登録する

# LINE Notifyサイトでの手順
手順が書かれたページを見つけましたので、[このページ](https://zenn.dev/protoout/articles/18-line-notify-setup)に従って、次のことを実施します。

1. LINE Notifyアカウントを自身のLINE友達に加える
1. アクセストークンを発行する

# 俺モニターでの手順

![通知](assets/img/LineNotify01.png)

![LINE Notify](assets/img/LineNotify02.png)

![アクセストークン](assets/img/LineNotify03.png)

![トークンの入力](assets/img/LineNotify04.png)

![送信テスト](assets/img/LineNotify05.png)

「送信」ボタンを押すと、LINE Notifyからメッセージが届くはずです。

![送信](assets/img/LineNotify06.png)
