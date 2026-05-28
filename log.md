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

## [2026-05-27] init | git init + GitHub push

- https://github.com/nishio/llm-wiki-about-nishio として公開

## [2026-05-27] ingest | サイボウズ + AI/LLM/機械学習 + word2vec

- `sources/サイボウズ-search.md` — サイボウズ42 + Cybozu 8 = 50件。Cybozu vs サイボウズ の表記使い分けを観察
- `sources/AI-LLM-機械学習.md` — 3語(536/98/17件)が同心円的に異なる射程で使い分けられていることを実証。`AIではなく機械学習.md` のメタページが本人の用語感覚を直接示す
- `sources/word2vec-自然言語処理.md` — 2014年著書周辺、word2vec×KJ法 がブロードリスニングへの長い系譜の起点
- `index.md` を更新

## [2026-05-27] ingest | コーディングを支える技術 + 未踏 + Scrapbox + KJ法

- `sources/コーディングを支える技術-search.md` — 7件のみ、エンジニアの知的生産術周辺50件と比して薄い→重心移動の数値証拠
- `sources/未踏-search.md` — 77件、2002〜2025の23年スパン、未踏ジュニア継続中、「未踏性」の理論化系
- `sources/Scrapbox-search.md` — 310件、基盤×研究対象の二重位置、派生ツール(AutoTrans/Connector/GPT)並走停滞
- `sources/KJ法-search.md` — 89件、60年スパンの方法論的核(物理→word2vec→Scrapbox→Kozaneba→AIでKJ法→ConnectingDots)

## [2026-05-27] filing-back | 概念2件 + 年/10年俯瞰

- `wiki/concepts/曖昧な停滞.md` — 出典 `行き詰まった協働と曖昧な停滞.md`、4スケール同型、Wiki内停滞事例も収録
- `wiki/concepts/ConnectingDots.md` — Dot粒度保留、KJ法系譜の最新位置
- `wiki/syntheses/年・10年スケール俯瞰.md` — 継続軸4本(知的生産レトリック/サイボウズ18年/未踏23年/KJ法系譜60年) + 10年区分3期 + 同じ問いの再実装3トラック + 用語の世代交代マップ

## [2026-05-28] ingest | Kozaneba + Keichobot

- `sources/Kozaneba-search.md` — 116件、2021-08起動の自作デジタル文房具、「一次元化フェーズ」
- `sources/Keichobot-search.md` — Keicho(68)+Keichobot(42)、2019年起動のチャットボット、「言語化フェーズ」。**LLM以前から(2019)同じコンセプトを実装、2023-03にGPT統合**
- `wiki/projects/Kozaneba.md` / `Keichobot.md` — 初の projects/ ページ
- 重要発見: **Keichobot=言語化 / Kozaneba=一次元化** という分業設計が `Keichobotは言語化しKozanebaは一次元化する.md` に明示。知的生産プロセスを2フェーズに分解

## [2026-05-28] filing-back | 未踏性 概念ページ

- `wiki/concepts/未踏性.md` — 個人×構造×動学の3層整理
  - 個人レベル: 自発的動機×新しさ（`未踏性とは.md`）
  - 構造レベル: 社会関係資本の集中、密小コミュニティのネットワーク（2011年論考）
  - 動学レベル: 課題感→協働→社会実装→イノベーション（2020〜2023の4世代継続改訂）
- 停滞TODO「Revisedネットワーク形成システムとしての未踏」が2011年以降**15年保留**であることを明示、改訂叩き台の素材を1ページに集約
