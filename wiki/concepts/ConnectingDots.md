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
- [[../../sources/KJ法-search.md|KJ法]] — 同じ原型操作の長い系譜
- [[../../sources/Scrapbox-search.md|Scrapbox]] — 既存の Dot 実装
- [[../topics/ブロードリスニング.md|ブロードリスニング]] — 集団スケールの Dot 配置

## Open Questions

- 外部脳内に `ConnectingDots` 名義の文書が他にあるか（要追加サーベイ）
- 既存ツール（Kozaneba, Scrapbox）と ConnectingDots の関係は、置換か / 上位レイヤーか / 別物か
- スティーブ・ジョブズの "connect the dots backwards" モチーフはどこまでロード bearing か、それとも語感だけか
- Dot 粒度を**用途ごとに切り替える**設計（固定しない）も選択肢として検討されているか
