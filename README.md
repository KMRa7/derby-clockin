# 🏇　ダービー 勤怠管理システム

## セットアップ手順

### 1. リポジトリ名を設定

`vite.config.js` の `base` をGitHubのリポジトリ名に合わせて変更してください。

```js
// 例: リポジトリが https://github.com/yourname/udon-app の場合
base: '/udon-app/'
```

### 2. GitHub Pages を有効化

GitHubリポジトリの **Settings → Pages** を開き、  
Source を **GitHub Actions** に設定してください。

### 3. pushするだけで自動デプロイ

```bash
git add .
git commit -m "init"
git push origin main
```

`main` ブランチにpushするたびに自動でビルド＆デプロイされます。

---

## ローカル開発

```bash
npm install
npm run dev
```

## アカウント情報（初期設定）

| 種別 | ユーザー名 | パスワード |
|------|-----------|-----------|
| 管理者 | admin | udon2024 |
| スタッフ | tanaka / sato / suzuki / yamada / ito | 1234 |

> ⚠️ パスワードは `src/App.jsx` 内の `ADMIN` と `INITIAL_STAFF` で変更できます。
