# apm-handson

Zenn 記事「Agent Package Manager (APM) をハンズオンで触ってみる」の手順を再現できるリポジトリです。

## 再現手順

```bash
# 1. APM CLI をインストール
curl -sSL https://aka.ms/apm-unix | sh

# 2. clone して install
git clone https://github.com/ry0y4n/apm-handson.git
cd apm-handson
apm install
```

`.github/instructions/`, `.github/prompts/`, `.github/agents/`, `.github/skills/` に
`microsoft/apm-sample-package` の primitive が配置されます。

## CI (apm audit)

`apm audit --ci --policy org` を GitHub Actions で実行し、組織の `apm-policy.yml` に基づいてポリシー違反を検知します。
詳細は Zenn 記事を参照してください。
