# Gmail ラベル一覧表示スクリプト

## 概要
このスクリプトは、Gmail APIを使用して、指定されたアカウントのGmailラベルを一覧表示します。

## 前提条件
- Python 3.x がインストールされていること
- `googleapiclient`, `google_auth_oauthlib` ライブラリがインストールされていること

## 使用方法
1. Google Cloud Platform で新しいプロジェクトを作成し、Gmail APIを有効にします。
2. OAuth 2.0 クレデンシャルをダウンロードし、`path/to/credentials.json` に保存します。
3. スクリプト内の `CREDENTIALS_PATH` を2でダウンロードしたファイルパスに更新します。
4. スクリプトを実行すると、ブラウザが開き認証を求められます。認証後、トークンが `path/to/token.pickle` に保存されます。
5. スクリプトは指定されたGmailアカウントのラベルを一覧表示します。

## 注意
- `token.pickle` および `credentials.json` は機密情報を含むため、公開場所にアップロードしないでください。

---
# Gmail Labels Listing Script

## Overview
This script uses the Gmail API to list the labels of a specified Gmail account.

## Prerequisites
- Python 3.x installed
- `googleapiclient` and `google_auth_oauthlib` libraries installed

## How to Use
1. Create a new project on Google Cloud Platform and enable the Gmail API.
2. Download OAuth 2.0 credentials and save them to `path/to/credentials.json`.
3. Update `CREDENTIALS_PATH` in the script to the path where you saved your downloaded file in step 2.
4. When you run the script, a browser will open asking for authentication. After authentication, the token will be saved to `path/to/token.pickle`.
5. The script will then list the labels of the specified Gmail account.

## Caution
- Do not upload `token.pickle` and `credentials.json` to public places as they may contain sensitive information.
