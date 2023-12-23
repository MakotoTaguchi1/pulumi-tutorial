# pulumi-tutorial

参考: https://dev.classmethod.jp/articles/pulumi-aws-tutorial-yaml/

# quickstart

・AWS pulumi用IAMユーザ作成
・クレデンシャル取得
・AWS CLIインストール

```
$ aws configure
$ mkdir quickstart && cd quickstart
$ pulumi new aws-yaml
$ pulumi up
→ details の後、 yes

少し修正して変更
$ pulumi up
$ pulumi stack output bucketName

リソース削除
$ pulumi destroy
```


# aws eks

```
$ mkdir eks && cd eks
$ pulumi new aws-yaml
This command will walk you through creating a new Pulumi project.

Enter a value or leave blank to accept the (default), and press <ENTER>.
Press ^C at any time to quit.

project name (eks):  
project description (A minimal AWS Pulumi YAML program): EKS stack 
Created project 'eks'

Please enter your desired stack name.
To create a stack in an organization, use the format <org-name>/<stack-name> (e.g. `acmecorp/dev`).
stack name (dev):  
Created stack 'dev'

aws:region: The AWS region to deploy into (us-east-1): ap-northeast-1 
Saved config

Your new project is ready to go! ✨

To perform an initial deployment, run `pulumi up`

# pulumi AIでコード生成

$ pulumi up
→エラー

```