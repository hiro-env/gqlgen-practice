# gqlgen

## 起動手順
1.go run main.goにてサーバーを起動する

## 動作確認

1.ブラウザでhttp://localhost:8080へアクセスしする
1.データを登録する```mutation {
  addUser(name: "Alice", email: "alice@somemail.com") {
    name
    email
  }```
1.データを取得する```{
  getUser(name:"Alice") {
    name
    email
  }
}```
1.データを更新する```mutation {
  updateUser(name: "Alice", email: "alice@alicemail.jp") {
    name
    email
}```
