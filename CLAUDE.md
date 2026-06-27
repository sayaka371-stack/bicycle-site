# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## プロジェクト概要

自転車をテーマにしたシンプルなプロフィールサイト（HTML/CSS のみ、ビルドツール・JavaScript なし）。

## ファイル構成

- `index.html` — サイト唯一のページ。Header / About セクション / Bicycle セクション / Footer で構成。
- `stylesheet.css` — 全スタイルをここに記述。外部リセットCSS（ress）は CDN から読み込み。
- `img/` — 画像素材（mainvisual, about, bicycle1〜3, logo, favicon）

## CSS 規約

- コンテナ幅は `.wrapper` クラス（`max-width: 960px`、左右 4% padding、`margin: 0 auto`）で制御。
- ブランドカラー: `#183057`（ヘッダーロゴ背景）。
- レスポンシブは `@media screen and (max-width: 600px)` の単一ブレークポイント。600px 以下で About のフレックス方向と Bicycle リストを縦並びに切り替える。
- リセット CSS として [ress](https://unpkg.com/ress/dist/ress.min.css) を CDN で使用。

## 開発・確認方法

ビルドツール不要。ブラウザで `index.html` を直接開くか、VS Code の Live Server 拡張で確認。
