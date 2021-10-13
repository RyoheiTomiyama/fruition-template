# ʕ •́؈•̀) `fruition-template`

fruitionをGitHubで管理できるようにしたもの

ドキュメント通りだとCloudflareWorkersの中にしかコードが残らないので、Gitで管理できるようにした

## 🔋 Getting Started

create development.json

```sh
cp config/example.json config/development.json
vim config/development.json
```

```sh
npm run dev
```
### 👀 Publishing

need jq

```sh
brew install jq
```

```sh
cp config/example.json config/production.json
```

```sh
vim config/production.json

# Set CF_ACCOUNT_ID and CF_API_TOKEN
#  "CF_ACCOUNT_ID": "",
#  "CF_API_TOKEN": ""
```

```sh
npm run deploy
```