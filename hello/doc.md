## vscodeでデバッグできるようにする

### エクステンション

Live Serverの拡張機能をインストール

### 起動

Go Liveボタンでサーバー起動

### vsコードのデバッグ機能を使う

.vscodeフォルダにlaunch.jsonを作る
以下を書く（ポートはLive Serverに合わせる）
```json
{
  "version": "0.2.0",
  "configurations": [
    {
      "type": "chrome",
      "request": "launch",
      "name": "live server",
      "url": "http://localhost:5500",
      "webRoot": "${workspaceFolder}"
    }
  ]
}
```

### デバッグ

デバッグ起動ボタンでクロームを選択し動けばOK


### 参考

https://ics.media/entry/11356/