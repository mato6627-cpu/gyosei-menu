# ミライズ 行政書士メニュー プロジェクト

行政書士が顧客に導入してもらうLINE公式アカウントのメニューから開く「行政書士業務のご案内」ページ。
補助金ファインダー(https://hojokin-finder.pages.dev/)と同じデザインテイストのスマホ縦型ページ。

## メインファイル
- **`index.html`** — 業務一覧ページ(全30業務・8カテゴリー)
  - 〇が付いた業務のみ掲載。各業務に1〜2行の説明付き
  - 条件がある申請には「📌 主な条件」のオレンジ枠を表示
  - カテゴリータイルをタップすると絞り込み表示

## GitHub・公開
| 項目 | 内容 |
|---|---|
| GitHubアカウント | mato6627-cpu |
| GitHubリポジトリ | https://github.com/mato6627-cpu/gyosei-menu |
| 公開URL | https://gyosei-menu.pages.dev (Cloudflare Pages接続後に確定) |
| デプロイ | GitHub push → Cloudflare Pages 自動反映(1〜2分) |

## Git操作
```bash
# 通常のアップロード
git add index.html
git commit -m "変更内容の説明"
git push origin main

# pushが弾かれた場合
git pull origin main --no-rebase
git push origin main
```

## 注意
- 条件表示は一般的な目安に簡略化してある(自治体・業種で細部が異なる)。文言変更時は導入先の行政書士に確認してもらうこと
- 特定の事務所名は入れていない(複数の行政書士事務所で使い回す前提)
