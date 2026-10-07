---
type: project
summary: nhiro.org（nishio/entrypoint）の情報設計と運用規約。2026-07-28〜29 に旧VPSからGitHub Pagesへ完全移行し、名刺+Story+凍結アーカイブの3層構造で刷新
sources:
  - 本人との対話 session（2026-07-28〜29, grasp-nishio）
  - https://github.com/nishio/entrypoint
---

# entrypoint (nhiro.org)

本人公式サイト。2012年契約のさくらVPS（Ubuntu 12.04, EOL）から GitHub Pages へ 2026-07-28〜29 に完全移行し、同時に情報設計を刷新した。リポジトリ: `nishio/entrypoint`（public）、配信: `docs/`、独自ドメイン `nhiro.org`（HTTPS強制、www→apex 301、github.io→nhiro.org 301）。

## 情報設計（2026-07 本人と合意した構造）

3層構造:

1. **名刺（トップ）** — `index.html`（英）/ `ja.html`（日）。薄く保つ。目次にしない。
2. **Story（側面別の入口）** — 興味関心ごとのナラティブページ。「西尾という人格にはたくさんの側面があり、入り口はたくさんある」（本人）。現在3本: `broadlistening/`・`plurality/`・`intellectual-production/`（各 英`index.html`+日`ja.html`）。相互に「関連 Story」でリンクし、どの入口からも他の側面へ辿れる。
3. **凍結アーカイブ** — `langbook/` 等の旧コンテンツ。**当時の見た目のまま残す**（新旧の見た目の差がそのまま鮮度の層の可視化 =「陳腐化はバグでなく史料」）。

Story の書式: 定義 → なぜ取り組むか（本人の解釈フレーム引用）→ 実践の記録（**検証可能なリンク付き・日付入り Dot を時系列で**）→ ツール → もっと読む → 末尾に「YYYY-MM-DD 時点の記録。今後も追記される」の日付スタンプ。

## 参照モデル

- **Gendlin bio（focusing.org）** — 全著作が一箇所でカタログ化され、伝記的ナラティブが著作群を縫う。読者の関心ごとに別の入口。**死後も Institute が維持し思想がアクセス可能であり続けている = [[因果的不死]]の実例**として本人が参照。
- **[[ConnectingDots.md|ConnectingDots]]** — Story ページは「Dot を選んで線を編む」の手書き先行実装。Dot の価値は事前に分からないので**凍結規約のような早すぎる制約は入れない**（本人指摘）。生き残る不変条件は「由来が追えること」のみ（URL を動かすなら moved-here を残す転送の規律）。

## 運用規約（確立済み）

- ディレクトリの `index.html` = 英語、`ja.html` = 日本語（トップも Story も同じ規則）。hreflang で相互宣言。
- 導線は**上り優先**: 深い URL に着地した読者を「その Dot を文脈づける Story」へ上げる方が、トップからの下り目次より価値が高い。
- 公開物は `docs/` のみ（repo root の TODO.md 等は非公開）。ビルドなし・JSなしの手書き HTML + `static/site.css`（システムフォント・ダークモード・モバイル対応の約160行）。SSG は「自由な試行錯誤の妨げ」として本人が却下。
- 図版は外部サービスに hotlink せず自己ホスト（例: broadlistening の CC0「あの図」）。

## 残タスク（2026-07-29 時点）

- what_i_did/ のアーカイブ目録化（全ディレクトリの注釈付き一覧）
- `t/` のリネーム + moved-here スタブ
- entrypoint への CLAUDE.md 設置と Claude GitHub App 接続（remote-control 有効化）
- メール（MX は旧VPS向きのまま）の扱い決定 → VPS 解約
- 高解像度顔写真（サイト+DD2030フォーム共通のボトルネック）

## 関連

- [[../meta/目的-自己紹介ページ更新.md|第一目的: 自己紹介ページを更新する]] — このプロジェクトの司令塔
- [[../concepts/自己紹介と歴史は共通の構造を持つ.md|自己紹介と歴史は共通の構造を持つ]] — Story 構造の理論的根拠
- [[../topics/ブロードリスニング.md|ブロードリスニング]] / [[../topics/Plurality.md|Plurality]] / [[../topics/知的生産.md|知的生産]] — 3本の Story の素材元

## Updates

### 2026-10-07 lint（entrypoint の git log と TODO.md で確認）

- Story は 3 本から 5 本に増えた: 2026-08-01 に `mentoring/`・`highdim/` を追加。6 本目「Visual Thinking」は保留（TODO.md）
- ConnectingDots の crawl 面（`dots.json`、Dot/Story ごとのページ、sitemap）を `nhiro.org/connecting_dots/` 配下に配信。2026-10-05 時点で 97 Dot / 8 Story、CV View あり。ソースは `nishio/connecting_dots`
- 残タスクのうち完了: `entrypoint/CLAUDE.md` の設置、`t/` → `pdf/` のリネーム（2026-07-29）
- 残タスクのうち未完了: 高解像度顔写真（プレスキットのブロッカー）。what_i_did/ の目録化、Claude GitHub App 接続、MX と旧 VPS 解約の状態はこの lint では確認していない
- 肩書きの英語表記は TODO.md のプレスキット案で「Research Director, Cybozu Labs」
