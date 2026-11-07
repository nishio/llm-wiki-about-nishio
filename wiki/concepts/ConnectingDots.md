---
type: concept
summary: nishio が構想中のシステム。Dotの粒度設計を意思決定保留中。このLLM Wikiが粒度設計の前段として機能する想定
sources:
  - memory（本人発言の保存版）
  - raw/external_brain_in_markdown/pages/ConnectingDots* (1件、要詳細確認)
---

# ConnectingDots

nishio が構想中のシステム。スティーブ・ジョブズのスタンフォード演説「you can't connect the dots looking forward; you can only connect them looking backwards」に由来するモチーフ。

外部脳のファイル名一致は1件のみ（要詳細追加サーベイ）。本ページは主に本人の発言（メモリ由来）と、外部脳の関連概念から構築。

## 中核の問い

> Dotはどのような粒度であるべきか？

事前に決めるのではなく、**LLM Wiki に整理してから判断する** と本人が表明している。
→ ConnectingDots の Dot 粒度設計は **このLLM Wikiの間接的な成果物** として位置付けられている。

## 関連する原型操作

ConnectingDots は nishio の方法論の系譜上にある：

- **KJ法** — 断片(付箋)を空間配置して構造を発見する原型操作（[[../../sources/KJ法-search.md|KJ法サーベイ]]）
- **Scrapboxのリンクとカード** — デジタル化された Dot の集合
- **word2vec とベクトル空間** — Dot を統計的距離で配置する
- **Kozaneba** — KJ法の専用ツール、Dotの直接実装
- **ブロードリスニング** — 集団スケールの Dot 配置（百万人の意見クラスタリング）

→ **「Dotを集めて構造を見出す」操作は、nishio研究を貫く方法論の核**。ConnectingDots はその最新の名前。

## 粒度設計の難しさ（推測される論点）

- **Scrapboxページ**: 1ページ = 1 Dot とすると粒度が大きすぎる場合がある
- **Scrapboxの行/段落**: 細かすぎてコンテキストを失う
- **KJ法の付箋**: 物理的な紙面サイズが暗黙の制約
- **word2vecの単語**: 単位は明確だが意味のまとまりとしては小さい

→ どのレイヤーで Dot を切るかが固定されない（または用途ごとに切り替える必要がある）のが「粒度の問題」と推測。

## 「曖昧な停滞」事例としての位置

- Dot 粒度設計は**意思決定保留中**
- 意思決定のハンドルを保留したまま動かないと、ConnectingDots システム自体も動かない
- → [[曖昧な停滞.md|曖昧な停滞]] の典型事例
- → 本人の戦略は「**LLM Wikiにまとめてから粒度を判断する**」= AI に委ねる中継ぎ

## 関連

- [[曖昧な停滞.md|曖昧な停滞]] — Dot 粒度設計はこのフレームの事例
- [[始める-広げる-繋げる.md|始める / 広げる / 繋げる]] — 「点を打つ(A)→繋げる(C)」の方法論的基礎。本人自己評価 C>A>B が ConnectingDots を C 中心戦略として裏付ける
- [[AI協働の4パターン.md|AI協働の4パターン]] — D パターン（データソース間の結合発見）は ConnectingDots の AI 実装路線として読める
- [[../../sources/KJ法-search.md|KJ法]] — 同じ原型操作の長い系譜
- [[../../sources/Scrapbox-search.md|Scrapbox]] — 既存の Dot 実装
- [[../topics/ブロードリスニング.md|ブロードリスニング]] — 集団スケールの Dot 配置

## Open Questions

- ConnectingDots は独立した `connecting_dots` 実装として自己紹介 Dot の本移行を終えている（2026-08-01）。Kozaneba 接続は2026-10-07の実装照合で未着手。既存ツールとの実際の接続・役割分担は引き続き確認する。

## Updates

### 2026-10-07 lint: 「Dot 粒度は保留中」はもう現状ではない

- 実装は `nishio/connecting_dots`（public）、設計 wiki は connecting-dot-design。HANDOFF.md によれば設計は closed で、`build.py` が end-to-end で動いている
- Dot 粒度の問いは「Dot と Story は固定層でなく相対的な役で、Dot 粒度は出力（View）の高度が決める」（flatness-is-view-resolution）という形で決着した
- 2026-08-01 に自己紹介 Dot の本移行を終え、nhiro.org/connecting_dots/ で公開。2026-10-05 時点で 97 Dot / 8 Story
- したがって本文の「意思決定保留中」「曖昧な停滞の典型事例」は 2026-05 時点の記述。上の Open Questions のうち「外部脳内に ConnectingDots 名義の文書が他にあるか」以外は、connecting-dot-design 側で扱われている

- 2026-11-07: 解決済みとしてOpen Questionsから除外 — 外部脳内に `ConnectingDots` 名義の文書が他にあるか（要追加サーベイ）。ConnectingDots 名義の追加文書「価値観のボトムアップ言語化=氷山モデル=ConnectingDots」を原文で確認。既存文書の見落としの解消であり、新規作成や網羅調査完了を意味しない。（根拠: 公開 Cosense 本人本文、raw HEAD 3f386ee8（2026-06-09）、`/Users/nishio/llm-wiki-about-nishio/raw/external_brain_in_markdown/pages/価値観のボトムアップ言語化=氷山モデル=ConnectingDots.md:11`）
- 2026-11-07: Open Questionsの現状を更新 — 既存ツール（Kozaneba, Scrapbox）と ConnectingDots の関係は、置換か / 上位レイヤーか / 別物か。公開実装と手書きStoryからの本移行は確認できる。一方、Kozanebaとの接続は未着手で、GPTによる比較表を本人の確定判断とは扱わない。（根拠: connecting_dots 579bd66（2026-08-01）、`/Users/nishio/connecting_dots/HANDOFF.md:9`・`/Users/nishio/connecting_dots/HANDOFF.md:84`；29aa9ca・2026-10-07 の実装照合記録、`/Users/nishio/connecting-dot-design/wiki/open-questions.md:234`）
- 2026-11-07: 解決済みとしてOpen Questionsから除外 — スティーブ・ジョブズの "connect the dots backwards" モチーフはどこまでロード bearing か、それとも語感だけか。2026-08-01の本人対話が、既に打っている点を忘れないため記録するという動機を明記している。語感だけかという問いへの直接の根拠がある。（根拠: 2026-08-01 本人対話、`/Users/nishio/connecting-dot-design/wiki/concepts/connecting-dots.md:35`；2026-08-01 LOG（05ec541 に収録）、`/Users/nishio/connecting-dot-design/wiki/log.md:68`）
- 2026-11-07: 解決済みとしてOpen Questionsから除外 — Dot 粒度を**用途ごとに切り替える**設計（固定しない）も選択肢として検討されているか。2026-07-30の本人同意により、粒度は出力の高度が決め、DotとStoryは相対的な役と決定。再帰的表現を全て実装したという判定ではない。（根拠: 2026-07-30 decision LOG（05ec541 に収録）、`/Users/nishio/connecting-dot-design/wiki/log.md:117`）
