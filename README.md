# go-remote-container
https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers

goの環境をvscode-remote-containerで動かすもの

## ひつようなこと
- Dockerが動く環境であること
- VScodeが動く環境であること
- vscode-remote-containerの拡張機能がインストールされていること

## そのた
`Dockerfile`に自動補完等のツールを入れているが、必要でないならコメントアウトすること

## きどうのしかた
- `./go-remote-container`の中に`main.go`などを入れる(ディレクトリを作成し、その中へファイルを入れる場合は`docker-compose.yaml`の`volumes`を変更すること)

```
.
|── .devcontainer
|  |──  devcontainer.json
├── Dockerfile
├── README.md
├── docker-compose.yaml
├── go.mod
├── go.sum
└── main.go
```
- `F1`キーを押し、`Remote-Containers: Rebuild Container`を押す(初回起動のみ、次回からはビルドはしてくても良い)
- ターミナルで好きなことをする、がんばる
