# CloudFormation実行ロール
  CloudFormationで環境を作るにあたって、以下のロールをAWS CLIで作成する。  
  ※cfnの実行自体に必要なので、これはcfnでのIaC管理外になる。

  * cfn-gitaccess-role:  cfnからテンプレートを置くgithubにアクセスするためのロール
  * cfn-execte-role:     cfnから各AWSサービスを起動するためのロール

  cloudshellで以下のコマンドを実行してロールを作成する。  
  ```
  aws iam create roll -f {テンプレートファイル名}
  ```
