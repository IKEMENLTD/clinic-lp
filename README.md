# Re:Design Clinic LP

オンライン診療（医療ダイエット・ピル・美容内服・エクソソーム・ED・AGA）のランディングページ。

## 構成

- `index.html` — 単一ページ。CSS/JS込み。ビルド不要の静的サイト
- `assets/img/` — 画像一式（ロゴ・カテゴリ写真・商品写真・診療フロー図）

商品データ（価格・効果・副作用・定期購入プラン）は `index.html` 内の `groups` オブジェクトに集約。価格改定・商品追加はここを編集する。

## 画面遷移

ハッシュルーティングで擬似ページ遷移する。

- `#cat-p_xxx` — カテゴリ一覧（例: `#cat-p_himan`）
- `#product-xxx` — 商品詳細（例: `#product-manjaro-25`）
- `#teiki` — 定期購入ページ

## デプロイ

静的ホスティング（Netlify / GitHub Pages 等）にそのまま配置可能。
