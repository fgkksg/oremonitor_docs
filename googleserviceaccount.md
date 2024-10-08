---
title: スプレッドシートを編集できるようにする
description: 俺モニターがGoogleスプレッドシートを編集できるようにする手順を説明します。
---

目次

1. [はじめに](#introduction)
1. [Google Cloudコンソールでの手順](#googlecloudconsole)
1. [Googleスプレッドシートでの手順](#googlespreadsheet)
1. [俺モニターでの手順](#oremonitor)

---

<a id="introduction"></a>

# はじめに
**俺モニター**がGoogleスプレッドシートを編集できるようにするために、**Googleサービスアカウント**を利用します。

大まかな手順の説明です。

1. **Googleサービスアカウント**を作成する（無料で作れます）
1. Googleスプレッドシート用のAPIを有効化する
1. **Googleサービスアカウント**の鍵を作成する
1. 作成した**Googleサービスアカウント**をGoogleスプレッドシートの共有ユーザーに追加する
1. **Googleサービスアカウント**の鍵を**俺モニター**に登録する

---

<a id="googlecloudconsole"></a>

# Google Cloudコンソールでの手順

## Google Cloudコンソールにログイン
[Google Cloudコンソール](https://console.cloud.google.com/welcome)にGoogle個人アカウントでログインします。

![ログイン画面](assets/img/GoogleCloudConsole01.png)

## プロジェクトを作成
任意のプロジェクトを作成します。

![プロジェクトを作成1](assets/img/GoogleCloudConsole02.png)

![プロジェクトを作成2](assets/img/GoogleCloudConsole03.png)

## スプレッドシートAPIの有効化
プロジェクトのスプレッドシートAPIを有効化します。

### プロジェクトの選択
先ほど作成したプロジェクトを選択します。

![作成したプロジェクトの選択](assets/img/GoogleCloudConsole04.png)

### スプレッドシートAPIを探して有効化
プロジェクトの中からスプレッドシートAPIを探して有効化します。

![APIとサービスのメニューを選択](assets/img/GoogleCloudConsole05.png)

![APIとサービスを有効にする](assets/img/GoogleCloudConsole05a.png)

![スプレッドシートAPIを探す](assets/img/GoogleCloudConsole05b.png)

![スプレッドシートAPIが見つかる](assets/img/GoogleCloudConsole05c.png)

![スプレッドシートAPIを有効にする](assets/img/GoogleCloudConsole05d.png)

## Googleサービスアカウントの作成
**俺モニター**に使わせる**Googleサービスアカウント**を作成します。

### サービスアカウントの作成

![認証情報のメニューを選択](assets/img/GoogleCloudConsole06.png)

![サービスアカウントを選択](assets/img/GoogleCloudConsole07.png)

![サービスアカウント名を入力](assets/img/GoogleCloudConsole08.png)

下の図では「参照者」を選択していますが「オーナー」でもOKです。「閲覧者」や「編集者」でも大丈夫かも知れません（詳しく分かっていません）。

![ロール（役割）を選択](assets/img/GoogleCloudConsole09.png)

![完了](assets/img/GoogleCloudConsole10.png)

### 鍵の作成とダウンロード
**俺モニター**に読み込ませるための鍵を作成します。

![サービスアカウントの選択](assets/img/GoogleCloudConsole11.png)

![キーの選択](assets/img/GoogleCloudConsole12.png)

![新しい鍵を作成](assets/img/GoogleCloudConsole13.png)

![鍵のダウンロード](assets/img/GoogleCloudConsole14.png)

保存したファイルはパスワードが書かれたファイルのようなものなので、公開しないでください。後で**俺モニター**に読み込ませます。

![保存](assets/img/GoogleCloudConsole15.png)

後でGoogleスプレッドシートの共有設定で入力するので、メールアドレスを控えておきます。

![メールアドレスの保管](assets/img/GoogleCloudConsole16.png)

---

<a id="googlespreadsheet"></a>

# Googleスプレッドシートでの手順
Googleスプレッドシートを共有に設定し、**Googleサービスアカウント**を共有ユーザーに追加します。

## スプレッドシートを共有に設定する
任意のGoogleスプレッドシートを作成し、**俺モニター**と共有できるようにします。

![共有設定](assets/img/GoogleCloudConsole17.png)

![サービスアカウントのメールアドレスを入力](assets/img/GoogleCloudConsole18.png)

## スプレッドシートのIDをコピーする
**俺モニター**に設定するために必要なスプレッドシートIDを控えておきます。

![スプレッドシートID](assets/img/GoogleCloudConsole19.png)

---

<a id="oremonitor"></a>

# 俺モニターでの手順

ダウンロードした鍵ファイルを**俺モニター**に登録します。

![設定を選択](assets/img/OreMonitor01.png)

![認証を選択](assets/img/OreMonitor02.png)

![Googlサービスアカウントを選択](assets/img/OreMonitor03.png)

![鍵の読み込みを選択](assets/img/OreMonitor04.png)

![ファイルを選択](assets/img/OreMonitor05.png)

![成功](assets/img/OreMonitor06.png)
