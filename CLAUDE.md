## このプロジェクトの目的

**西尾泰和（nishio）自身**についての LLM-Wiki。

外部脳（Scrapbox `nishio` から書き出された Markdown 群、24,000+ ページ）を一次ソースとし、本人による知的生産の流れ・関心領域・概念・プロジェクトを整理する。本人が見落としがちな **年スケール・10年スケールの視点** を浮かび上がらせること、および **派生成果物（自己紹介ページ、ConnectingDots、停滞している意思決定への助言）の土台** を提供することを狙う。

> 公開版。非公開ソース（個人ジャーナル等）を含む派生Wikiは別途。

## ディレクトリ構成

- [raw/](raw) — 生ソース。読み取り専用。改変しない。
  - [raw/external_brain_in_markdown/](raw/external_brain_in_markdown) — Scrapbox `nishio` の Markdown エクスポート（git clone, gitignored, `git pull` で更新可）
- [wiki/](wiki) — Wiki 本体
  - [wiki/concepts/](wiki/concepts) — 西尾の造語・特定用法の概念ページ（例: `ConnectingDots`、`曖昧な停滞`、`知的生産` の本人的フレーミング）
  - [wiki/topics/](wiki/topics) — 関心テーマのエントリーページ（例: `知的生産`, `ブロードリスニング`, `Plurality`, `AI×人文`）
  - [wiki/projects/](wiki/projects) — プロジェクトページ（例: `Plurality-LLM-Wiki`, `Delite-LLM-Wiki`, `Policy-PR-Hub`）
  - [wiki/syntheses/](wiki/syntheses) — 統合解説・入り口ページ（自己紹介、「これは何？」、年/10年スケール俯瞰）
  - [wiki/meta/](wiki/meta) — Wiki 編集方針・マッピング
- [sources/](sources) — キーワード検索バンドル等の要約ページ
- [index.md](index.md) — Wiki 全体の索引
- [log.md](log.md) — ingest / query / lint の時系列ログ

### 新規ページをどこに置くか

| ページ種別 | 置き場所 |
|---|---|
| 西尾自身の造語・特定用法の用語 | `wiki/concepts/` |
| 関心テーマの入り口（複数記事をまとめる枠） | `wiki/topics/` |
| 具体的なプロジェクト | `wiki/projects/` |
| 「これは何？」「自己紹介」「年スケール俯瞰」など複数ページの統合解説 | `wiki/syntheses/` |
| Wiki の編集方針・マッピング | `wiki/meta/` |

## ページ規則

### 全ページ共通

- 冒頭にYAMLフロントマター: `type`, `summary`, `sources`
- 主張には出典を明記: `[[source名]]より` または ファイルパス
- 矛盾・未解決の論点は `## Open Questions` で明示
- 更新は上書きせず `## Updates` で追記

### フロントマター例

```yaml
---
type: concept
summary: 1文で説明
sources:
  - 知的生産-search.md
---
```

### typeの種類

- `concept` — 造語・概念・特定用法
- `topic` — 関心テーマの入り口
- `project` — プロジェクト
- `synthesis` — 統合解説・入門・俯瞰
- `meta` — Wiki 編集に関する話

## ワークフロー

### Ingest（キーワード駆動）

24,000+ ページを一気には扱えないため、**キーワードで切り出して束ね、要約して、束のソース要約を残す** スタイルで進める。

1. キーワード（例: `知的生産`）で `raw/external_brain_in_markdown/pages/` を `grep` し、ヒットしたページのリストを得る
2. [sources/](sources) に `<キーワード>-search.md` を作り、ヒット件数・代表ページ・読み取った要点を要約
3. 概念・テーマ・プロジェクトに該当するページが新出なら `wiki/` に追加または既存ページを更新
4. [index.md](index.md) を更新
5. [log.md](log.md) に `## [YYYY-MM-DD HH:MM] ingest | <キーワード or 範囲>` を追記

### Query

1. [index.md](index.md) を起点に関連ページを探す
2. 必要に応じて `raw/` も検索
3. 有用な発見は `wiki/syntheses/` に filing back
4. [log.md](log.md) に `## [YYYY-MM-DD HH:MM] filing-back | <description>` を追記

### Lint

定期的に health-check:

- 孤立ページ・壊れたリンク・index 未登録の検出
- 概念ページなのにソースが書かれていないものの検出
- ソースで言及されているのに概念ページが無い用語の検出
- stale な「最新状況」記述の検出（年/10年スケール俯瞰では特に注意）

## 編集方針

- ソース（Scrapbox エクスポート）の本人テキストを最重視する
- 時系列の文脈を保つ。Scrapboxページの作成日・更新日・タグを利用して **いつ頃の関心だったか** を明示する
- 既に乗り越えた過去の考え方と、現在進行形の関心を区別する
- 推測で書く部分は明示する（「と思われる」「不明」など）
- **年/10年スケール俯瞰** を作る際は単一ページ依存にしない（複数ページの突き合わせで根拠を作る）
