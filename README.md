# gqlgen

## 起動手順
1.`go run main.go`にてサーバーを起動する

## 動作確認

**1.ブラウザでhttp://localhost:8080へアクセスする<br>**

**2.データを登録する**

```
mutation {
  addUser(name: "Alice", email: "alice@somemail.com") {
    name
    email
  }
}
```

**3.データを取得する**

```
{
  getUser(name:"Alice") {
    name
    email
  }
}
```

**4.データを更新する**

```mutation {
  updateUser(name: "Alice", email: "alice@alicemail.jp") {
    name
    email
  }
}
```
