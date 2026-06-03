# AI活用診断誘導LP

中小企業の経営層向けに、AI活用レベル無料診断ページへ遷移してもらうためのNext.js LPです。

## 構成

- Next.js App Router
- TypeScript
- 1ページ完結型LP
- 問い合わせフォームなし
- 全CTAは診断ページへ遷移

## 起動

```bash
npm install
npm run dev
```

## ビルド

```bash
npm run build
```

## 診断ページ

全CTAは以下へ遷移します。

https://ai-qaw7.vercel.app/

## 主な編集箇所

- LP本文・リスト: `app/page.tsx`
- SEO title / description: `app/layout.tsx`
- デザイン調整: `app/globals.css`
- ヒーロー画像: `public/images/ai-executive-hero.png`

## GitHubへ取り込む対象

以下をリポジトリルートとしてそのままGitHubへ追加できます。

```text
app/
public/
.gitignore
README.md
next-env.d.ts
next.config.ts
package.json
tsconfig.json
vercel.json
```

## GitHubアップロード手順

1. ZIPを使う場合は、ZIPファイル自体をGitHubに置くのではなく、解凍した中身をアップロードしてください。
2. GitHubのリポジトリ直下に `app/`, `public/`, `package.json` が見える状態にしてください。
3. Vercelに接続する場合は、Framework Presetを `Next.js` にしてください。
