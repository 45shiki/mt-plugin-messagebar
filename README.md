# MessageBar プラグイン

## 概要

管理画面の上部に固定のメッセージを表示する

## 動作環境

- Movable Type 6
- PowerCMS 4

## インストール

1. ZIP アーカイブ *MessageBar.zip* を解凍し、サーバ上のプラグインディレクトリへ *MessageBar* を設置する

    例 :

        $MT_HOME/plugins/MessageBar

    ※ `$MT_HOME` は CMS のインストール先を指します

1. 管理画面へログインする
1. システムレベルのプラグイン設定の一覧に MessageBar が表示されていることを確認する

## 設定

設定はシステムレベルのプラグイン設定と環境変数の双方から行えます。
MessageBar の設定では以下の特徴があります。

- プラグイン設定と環境変数のどちらも設定している場合は環境変数の設定が使われます
- 環境変数を設定している場合、プラグイン設定は入力できません
- プラグイン設定`文字色`と`背景色`にはデフォルト値があります
- 環境変数 `MessageText` とプラグイン設定`テキスト`の両方が未設定の場合は管理画面のホスト名 (`****.jp`) が表示されます

### プラグイン設定


- テキスト

    表示するメッセージを指定します。

- 文字色

    メッセージの文字色を CSS の color プロパティと同様のフォーマットで指定します。 (デフォルト値: `#ffffff`)

- 背景色

    メッセージの背景色を CSS の background-color プロパティと同様のフォーマットで指定します。 (デフォルト値: `#c53d43`)

### 環境変数

- MessageText

    表示するメッセージを指定します。マルチバイトで指定する場合は UTF-8 で記述します。

        MessageText  ここはテスト環境です

- MessageTextColor

    メッセージの文字色を CSS の color プロパティと同様のフォーマットで指定します。

        MessageTextColor  #ffffff

- MessageBackgroundColor

    メッセージの背景色を CSS の background-color プロパティと同様のフォーマットで指定します。

        MessageTextColor  #c53d43

## 使い方

特別な操作は必要ありません。管理画面へアクセスすると画面の上部に固定のメッセージが表示されます。

## 更新履歴

- ver.0.45 (2018年03月26日) 公開

## 奥付
- Alfasado Inc.
- https://alfasado.net/
- 2018年03月26日
