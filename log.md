# Log

時系列の作業記録。新しいものを下に追記する。

## [2026-05-27] scaffold | 初期セットアップ

- `/Users/nishio/llm-wiki-about-nishio/` を作成
- デライト版（[llm-wiki-about-delite](https://github.com/nishio/llm-wiki-about-delite)）のパターンを参考に、subject が西尾自身であるという違いに合わせて構造を調整
- `raw/external_brain_in_markdown/` に Scrapbox `nishio` の Markdown エクスポートを clone（24,921ファイル, 164MB, gitignored）
- 初期 ingest はキーワード駆動（`知的生産`, `ブロードリスニング`, etc.）で進める方針

## [2026-05-27] ingest | 自己紹介bios + 知的生産115件 + 入り口/三大テーマ

- `sources/自己紹介-bios.md` — 自己紹介ページの時系列bio分析、関心の変遷を5期に整理
- `sources/知的生産-search.md` — 115件を8クラスタ（著書本体周辺/続編/概念/AI×/方法論/集団/他流派/停滞TODO）にクラスタリング
- `wiki/syntheses/これは何？.md` — Wikiの入り口。「これは何か」「nishioとは何者か」を5期テーブルで提示
- `wiki/topics/知的生産.md`, `ブロードリスニング.md`, `Plurality.md` — 三大テーマのエントリーページ
- `index.md` を更新

## [2026-05-27] filing-back | 初回ingestから見えたパターンと未着手ページ案

- `wiki/syntheses/nishio観察パターン.md` — 7つの横断パターン（固定軸+射程拡大 / ブリッジ言語 / これは何？の主語ずれ / NEXT本並走 / 停滞TODO可視化 / AI生成レイヤー混在 / 外部公開bioのメンテ放置）
- `wiki/meta/proposed-next-pages.md` — 曖昧な停滞、ConnectingDots、年/10年スケール俯瞰の3案を実行待ち
