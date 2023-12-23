# pulumi-tutorial

参考: https://dev.classmethod.jp/articles/pulumi-aws-tutorial-yaml/

# quickstart

・AWS pulumi用IAMユーザ作成
・クレデンシャル取得
・AWS CLIインストール

```
$ aws configure
$ mkdir quickstart && cd quickstart
$ pulumi new aws-yam
$ pulumi up
→ details の後、 yes

少し修正して変更
$ pulumi up
$ pulumi stack output bucketName

リソース削除
$ pulumi destroy
```
