# first-frontend-development

## Github
https://github.com/okachijs/jsframeworkbook


## Firebase project
admin@howdylikes.jp

https://console.firebase.google.com/project/first-frontend-development/overview

## chat-server 
### functions
#### サーバー起動
```
firebase serve --only functions
```

#### デプロイ
```
firebase deploy --only functions
```

#### channel 登録
```
curl http://localhost:5000/first-frontend-development/us-central1/v1/channels -H 'Content-Type: application/json' -d '{"cname": "general"}' 
```

#### channel 一覧取得
```
curl http://localhost:5000/first-frontend-development/us-central1/v1/channels
```

#### message 登録
```
curl http://localhost:5000/first-frontend-development/us-central1/v1/channels/:cname/messages -H 'Content-Type: application/json' -d '{"body": "こんにちは！"}' 
```

#### message 一覧取得
```
curl http://localhost:5000/first-frontend-development/us-central1/v1/channels/:cname/messages
```

#### データリセット
```
curl http://localhost:5000/first-frontend-development/us-central1/v1/reset -H 'Content-Type: application/json' -d '{}'
```
