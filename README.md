# kagoike_slack_bot

## ローカルテスト
```
docker compose up --build -d
ngrok http 3000
```
SlackにURLを貼り付ける．エンドポイントは`slack/events`

## デプロイ
arm64でデプロイしないとjiter.jiterのimport errorが起きる．（原因不明）
dockerizePipを使うのでdockerを起動
```
serverless deploy
```