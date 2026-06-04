---
type: source-summary
summary: TODO:自己紹介ページを更新する を起点とした 26 ページの 2hop バンドル要約。停滞の構造、本人指針、Dots/Stories/Views 構造設計、entrypoint 実装、自己紹介ポーカー、すべての発言は自己紹介、までを横断的に整理
sources:
  - raw/nishio-todo_自己紹介ページを更新する.2hop.txt
---

# TODO:自己紹介ページを更新する 2hop バンドル要約

## バンドル構成

メイン 1 ページ + 1hop 7ページ + 2hop 18ページ = 26ページ。

## メインページ時系列（2026-01-20〜2026-02-17）

| 日付 | 内容 |
|---|---|
| 2026-01-20 | 開始。`nhiro.org/ja.html` が古いまま検索ヒット。3年間の活動が世界から関心持たれるゾーンへ |
| 2026-01-24 | nhiro.org 更新方法を発掘。entrypoint リポジトリ作成、GitHub Pages プレビュー |
| 2026-02-05 | [[../raw/external_brain_in_markdown/pages/AIに星占いをさせる.md|AI星占い]]経由で **5つの方針**腹落ち（完成版を作らない / 何者かより何を考えているか / 過去の自分を消さない / 2026夏以降に固まる / 名刺ではなく作業ログの入口） |
| 2026-02-11 | **ひらめき**: 「[[../wiki/concepts/自己紹介と歴史は共通の構造を持つ.md|自己紹介と歴史は共通の構造を持つ]]」 |
| 2026-02-17 | 「全然捗ってない、出力を見るのはした」 |
| 2026-02-22 | 週記: 「データとシステムを同時に作ったからビミョい」「自分で操作している感がなくなる」 |
| 2026-03-27 | [[../raw/external_brain_in_markdown/pages/ConnectingDotsシステム.md|ConnectingDotsシステム]] に接続 |

## 2026-02-11 のひらめき（Sonar 対話 25 問）

[[../raw/external_brain_in_markdown/pages/自己紹介と歴史は共通の構造を持つ.md|自己紹介と歴史は共通の構造を持つ]] で AI(Sonar) と 25 問の対話を行い、構造を引き出した。主要回答:

| Q | 本人回答 |
|---|---|
| 連帯の系譜? | 細かい個別事実の記録が振り返り時に Connecting Dots する |
| 動的生成? | 活動履歴を溜め、何をストーリーとして見せるかは人間のキュレーション |
| 微細な事実? | 価値は事前にわからないので微細でも記録 |
| 翻訳ではなく文脈最適化? | カード元データは再利用可能、ストーリーは文脈ごとに複数 |
| 私と公の両方? | どちらにも使えるシステムだ |
| 編集のしやすさ vs 正確性? | GitHub に置かれた JSON を想定 |
| Dot Connect の主体? | Dot を作った本人である必要はない |
| 言語別テンプレ? | **「これはアホの発想」**（テンプレではなく別編集の並立） |

→ Sonar が当初提案した「ジレンマ」「葛藤」を本人が否定し、最小限の構造へ収束:
- **Dots（点）** = 検証可能な最小単位、再利用可能、GitHub JSON
- **Stories（線）** = Dot を並べてコメントを添える「作品」、何本でも増える
- **Views（面）** = タイムライン / 人物別 / プロジェクト別の UI、薄く作れる

## GPT5 との続き対話（同ページ後半）

- 「薄さ」と「堅実さ」はジレンマじゃない（本人ツッコミ通り）
- 「収集の自動化」ではなく **「候補のインボックス化」**: 拾った候補(未確定) → Dots に昇格させるキュレーション編集 → Story
- 多言語は「テンプレ」ではなく「別編集の並立」（Plurality 本自体が型: gitベース、CC0、forkして自分版を作る）
- 自己紹介は「**ストーリーの 1 つ（Profile Story / Resume Story）**」、固定プロフィールは Story の表紙に退く
- dd2030 公式の「プロジェクトの歴史」が参考例: 週次レポートにリンクするだけの薄い構造、PR/Issue要約という堅実な粒度

→ つくる順番（最小実装）:
1. Dot のスキーマを薄く決める（date / refs / entities / verifiability）
2. Story のスキーマを自由度高く決める（dot_id 配列＋言語別 caption/note）
3. View を 1 個だけ（Story ページ）
4. 逆引き（dot → 含まれる stories）を自動生成

## 関連概念群（1hop / 2hop で展開）

### [[../raw/external_brain_in_markdown/pages/自己紹介.md|自己紹介.md]] (2017〜2026, 30+ bio が積層)
- 最新 (2026 未踏ジュニア用): Plurality 寄稿者・編集者・日本語化リーダー + ブロードリスニング事例
- 中期 (2024): TokyoTech 特定准教授退任、AI ブロードリスニング、シン東京2050
- 初期 (2008〜2018): エンジニアの知的生産術系、word2vec、サイボウズ・ラボ
- 本人発言: 「経歴(長いもの) http://nhiro.org/ja.html → メンテしてないな〜」

### [[../raw/external_brain_in_markdown/pages/自己紹介とポーカーの役.md|自己紹介とポーカーの役]] (2025-03-18)
- ノーペア vs 役を作る = 実績間の関連の見出し方
- 場ごとに強い役が異なる
- 目的設定: 際立つ / 際立たない / 仲間と認識される / 共通点を作る
- 4枚あっても無意味、5枚で初めて役になる
- 詳細は [[../wiki/concepts/自己紹介ポーカー.md|自己紹介ポーカー]]

### [[../raw/external_brain_in_markdown/pages/自己紹介の想定ユーザ.md|自己紹介の想定ユーザ]] (2023-05-17)
- 「すでに知ってる人は想定ユーザではない」
- 初手「ソフトウェアの会社で研究員」→ 食いつく相手だけに難しい話を返して 1bit 情報を得る

### [[../raw/external_brain_in_markdown/pages/自己紹介力.md|自己紹介力]] (2025-03-19)
- 自己紹介 ≠ 自己アピール ≠ セルフブランディング
- 「一人当たり 0.3 秒」のアテンション社会
- 詐欺師との対比: 特に何もしてないのにリソースくれる人は警戒

### [[../raw/external_brain_in_markdown/pages/すべての発言は自己紹介.md|すべての発言は自己紹介]] (2024-02-02)
- 「XはYだ」発言は「私は『XはYだ』と思ってる人です」の自己紹介
- 関連: [[../raw/external_brain_in_markdown/pages/悪口は自己紹介.md|悪口は自己紹介]]（ブーメラン構図）

### [[../raw/external_brain_in_markdown/pages/Self introduction in east Asian context.md|Self introduction in east Asian context]] (2023-04-22)
- 英語圏向け Mitou 解説テンプレ、Author/Artist セクション
- 未踏 / Mitou Foundation / Mitou Junior の解説あり
- 著書 4 冊（コーディング支援、word2vec、世界一わかりやすい、エンジニア知的生産術）

### [[../raw/external_brain_in_markdown/pages/ConnectingDotsシステム.md|ConnectingDotsシステム]] (2026-03-27〜04-26)
- 事実と解釈の明瞭分離
- 事実の集合は人間が読むには向かない、AIには有益
- 2026-04-26 設計 LLM Wiki `connecting-dots-design` を作成
- 「自己紹介ポーカー」が Story の本質を最も簡潔に言語化、と Karpathy LLM Wiki が判定

### [[../raw/external_brain_in_markdown/pages/事実の島の周りに解釈が広がっている.md|事実の島の周りに解釈が広がっている]] (2026-04-16)
- 事実 F の周囲に解釈が薄く広がる、まだ言語化されていない
- 連想 A はその薄く広がったところで起きる

## 並行 LLM Wiki プロジェクト群（[[../raw/external_brain_in_markdown/pages/日記2026-05-07.md|日記2026-05-07]] / [[../raw/external_brain_in_markdown/pages/複数のLLM_Wikiに共通のインプット.md|複数のLLM_Wikiに共通のインプット]]）

本人は複数の Karpathy LLM Wiki を並走させている:

| Wiki | 対象 |
|---|---|
| connecting-dots-design | ConnectingDotsシステムの設計 |
| LENCHI | LLMを使った知的生産（書籍プロジェクト） |
| ブロードリスニング本 | dd2030 連携 |
| KozanebaのLLM Wiki | 設計議論を集める（未着手） |
| 広聴AIのLLM Wiki | Google Docs 議事録（未着手） |
| 盲点カードLLM Wiki | VT 関連 |
| 注釈駆動Wiki | スマホ用 UI |
| **このWiki（llm-wiki-about-nishio）** | **nishio 本人** |

→ Wiki 同士が共通入力に対して異なる切り出しをする「**[[../raw/external_brain_in_markdown/pages/複数のLLM_Wikiに共通のインプット.md|wikis-as-personas]]**」の試行。MindTrellis 論文を 3 Wiki に投げて差分を比較した実験あり。

→ 本Wikiは「nishio 本人」というペルソナを担当。**自己紹介ページ更新が成果物**として接続される。

## 本人 2026-02-22 の困難分析

> データとシステムを同時に作ったからビミョい。どっちも8割くらいの完成度
> データを更新した時のプレビューをライブにして、満足いくデータに手で直す
> いま「最終的に静的HTMLを出力」と指示して、多分スクリプトで静的HTMLを出力するようになってると思う、把握してなくてCodexの中でブラックボックス
> 変更意図を伝えてから結果が返ってくるまでの時間が長くなって**自分で操作している感**がなくなる
> また直近に締切があるタスクを抱えている場合、レスポンスに時間のかかるリクエストを出したら、待たずに他のことをしてしまう
> これがコンテキストを寸断してしまう

→ **時間細切れ × 操作感欠如 × 並行締切タスク優先** という構造で停滞。
→ 本Wiki がコンテキストを Markdown ファイルとして提供することで「操作感」と「再開可能性」を担保できる可能性。

## 本Wikiの位置付け（このバンドルから明確化）

- 本人が「Dot 粒度設計を LLM Wiki にまとめてから」と明示した、その **LLM Wiki がこのWiki**
- entrypoint リポジトリ（ static HTML 出力先 / View 層）は別物として走らせる
- 本Wiki は **Dot 候補と Story の解釈語彙** を準備する側
- 詳細方針は [[../wiki/meta/目的-自己紹介ページ更新.md|目的-自己紹介ページ更新]]

## Open Questions

- entrypoint リポジトリの現状（8割完成と本人が認める）と本Wiki のページ群はどう接続するか
- Dot の JSON スキーマは本人と合意済か（バンドル内に最小要素提案あり: date / refs / entities / verifiability）
- 「2026年夏以降に名乗れる言葉が固まる」を待つべきか、暫定 Story を更新し続けるか
- 複数 LLM Wiki ペルソナの中で本Wikiが担うのは「本人 = nishio」のみか、それとも「自己紹介ページ更新」プロジェクトも兼ねるか
