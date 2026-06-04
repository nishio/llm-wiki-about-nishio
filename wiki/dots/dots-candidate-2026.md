---
type: dots-candidate
summary: 自己紹介ページ更新のための Dot 候補を、本人提案スキーマ(date/title/refs/entities/verifiability)で構造化。欠落Dot-2026.md を formalize したもの
sources:
  - wiki/syntheses/欠落Dot-2026.md
  - sources/todo自己紹介更新-2hop-bundle.md
  - raw/external_brain_in_markdown/pages/
---

# Dot 候補 一覧 2026

## このファイルの位置付け

[[../syntheses/欠落Dot-2026.md|欠落Dot-2026]] で識別した活動を、本人提案スキーマ（[[../../sources/todo自己紹介更新-2hop-bundle.md|todo自己紹介更新 2hop バンドル]] 内 GPT5 提案）で構造化したもの。

- 入力: 9 カテゴリの欠落 Dot
- 出力: 各 Dot に **date / title / refs / entities / tags / status / summary** を付与
- 用途: 本人 / Codex / entrypoint リポジトリへの import 候補。**ここは Dot 倉庫の前段（Inbox の出口）**

スキーマ（本人2026-02-11 GPT5 対話より）:

```
- date: いつ（YYYY-MM-DD or YYYY-MM or 期間）
- title: 何が起きたか（1行の主語＋述語）
- refs: 根拠リンク（URL または raw/.../*.md パス、最低1つ）
- entities: 関連する人・組織・タグ（任意）
- tags: カテゴリタグ（任意）
- status: confirmed / needs-date / ongoing / in-progress / planned
- summary: 1〜3行の説明
```

status の意味:
- **confirmed**: date と refs 両方検証済
- **needs-date**: refs あるが date が外部脳から特定できなかった
- **ongoing**: 継続中（固定日付なし、開始年のみ）
- **in-progress**: 執筆中・開発中など、完了未定
- **planned**: 着手意思のみ

---

## 1. 役職更新（bio に未反映または古い）

### D001 一般社団法人未踏 理事 退任
- **date**: 2025-05-13
- **refs**:
  - [[../../raw/external_brain_in_markdown/pages/一般社団法人未踏の理事を退任しました.md|raw: 一般社団法人未踏の理事を退任しました]]
  - https://x.com/nishio/status/1922128345287761959
- **entities**: 一般社団法人未踏, デジタル民主主義2030
- **tags**: 役職, 退任, 2025
- **status**: confirmed
- **summary**: 2015 年就任から 10 年で退任。社団との関係は良好、疎結合化の設計判断。同日チームみらい公式応援表明。

### D002 一般社団法人未踏 理事 在任期間
- **date**: 2015-06 〜 2025-05
- **refs**:
  - raw/external_brain_in_markdown/pages/一般社団法人未踏の理事に就任しました.md
  - D001 と同じ
- **entities**: 一般社団法人未踏
- **tags**: 役職, 期間
- **status**: confirmed
- **summary**: 10 年間理事を務めた。bio では「2015~2025」と期間表記すべき。

### D003 TokyoTech 特定准教授 退任
- **date**: 2024-03
- **refs**:
  - raw/external_brain_in_markdown/pages/自己紹介.md（「東京工業大学 特定准教授(2018/4~2024/3)」と本人記載）
- **entities**: 東京工業大学, 環境・社会理工学院, イノベーション科学系, 技術経営専門職学位課程
- **tags**: 役職, 退任, 2024
- **status**: confirmed
- **summary**: 2018-04 〜 2024-03 で 6 年。bio で在任期間として書く必要がある（2024-03 以降は「元」または期間明記）。

### D004 チームみらい 公式応援表明
- **date**: 2025-05-13
- **refs**:
  - https://x.com/nishio/status/1922134928554135939
  - https://team-mir.ai/
- **entities**: チームみらい, 安野貴博
- **tags**: 役職, 政治, 2025, disclaimer要
- **status**: confirmed
- **summary**: 未踏理事退任と同日に公式応援を表明。サイボウズの裁量労働で平日応援時は休みを取って業務外扱いの配慮あり。bio に書く場合は disclaimer 設計が必要。

### D005 サイボウズAIエキスパートチーム 兼務開始
- **date**: 2023
- **refs**:
  - raw/external_brain_in_markdown/pages/自己紹介.md（207文字版 bio）
- **entities**: サイボウズ, サイボウズ・ラボ
- **tags**: 役職, 兼務, 2023
- **status**: needs-date
- **summary**: 一部 bio にのみ記載。月日を本人に要確認。

### D006 デジタル民主主義2030 (dd2030) 主要メンバー
- **date**: 2025 ongoing
- **refs**:
  - raw/external_brain_in_markdown/pages/dd2030.md
  - raw/external_brain_in_markdown/pages/dd2030 slack.md
- **entities**: デジタル民主主義2030, dd2030
- **tags**: 役職, コミュニティ, ongoing
- **status**: ongoing
- **summary**: dd2030 slack 主要メンバー。広聴AI 開発の中心拠点。「世界を良くするために力を合わせたい人の集まり」と本人言及（D001 同日ツイート）。

---

## 2. ブロードリスニング案件（2024-2026、未踏ジュニアA bio から欠落）

### D101 シン東京2050 ブロードリスニング
- **date**: 2024 〜 2025-01-31（最終分析公開）
- **refs**:
  - raw/external_brain_in_markdown/pages/シン東京2050ブロードリスニング.md
  - https://www.metro.tokyo.lg.jp/tosei/hodohappyo/press/2025/01/31/09.html
  - https://x.com/nishio/status/1885274519830761611
- **entities**: 東京都, GovTech Tokyo, 安野貴博, Talk to the City
- **tags**: ブロードリスニング, 東京都, 政策, 2024, 2025
- **status**: confirmed
- **summary**: GovTech Tokyo アドバイザーの安野氏と共に東京都長期戦略策定にブロードリスニング協力。27,915 件の意見を Talk to the City 等で分析。一部ポリシーカテゴリが高解像度観察で複数クラスタに分割された。

### D102 都知事選2024 ブロードリスニング協力
- **date**: 2024-07
- **refs**:
  - raw/external_brain_in_markdown/pages/TTTC: 安野たかひろ都知事選出馬に関しての人々の反応と論点.md
  - raw/external_brain_in_markdown/pages/2024都知事選でのマイナ投票.md
- **entities**: 安野たかひろ, Talk to the City, TTTC
- **tags**: ブロードリスニング, 選挙, 都知事選, 2024
- **status**: confirmed
- **summary**: 安野たかひろ候補陣営の都知事選 2024 でブロードリスニング技術を活用。日本でこの概念が広く認知される契機。

### D103 日テレNEWS×2024衆院選×ブロードリスニング
- **date**: 2024-10-15 〜 2024-10-25
- **refs**:
  - raw/external_brain_in_markdown/pages/日テレNEWS×2024衆院選×ブロードリスニング.md
  - https://news.ntv.co.jp/category/society/1594a26c1d794967a9245ed34e70d681
  - https://note.com/annotakahiro24/n/ndd21a8ba3eec
- **entities**: 日本テレビ, 安野貴博, Talk to the City
- **tags**: ブロードリスニング, 選挙, 衆院選, メディア, 2024
- **status**: confirmed
- **summary**: 「地上波世界初」とされる、ブロードリスニング技術を使ったテレビ選挙報道。投票誰にする会議 〜みんなの声でつくる衆議院選挙2024〜。

### D104 JAPAN CHOICE 世論地図
- **date**: 2024-11
- **refs**:
  - raw/external_brain_in_markdown/pages/JAPAN CHOICE.md
  - raw/external_brain_in_markdown/pages/2024-11-14-世論地図のUMAP.md
- **entities**: Mielka, JAPAN CHOICE
- **tags**: ブロードリスニング, 政治, 2024
- **status**: confirmed
- **summary**: NPO 法人 Mielka の政治意思決定支援サイト「JAPAN CHOICE」の世論地図に協力。UMAP 可視化。

### D105 参院選2025 ブロードリスニング
- **date**: 2025-07
- **refs**:
  - raw/external_brain_in_markdown/pages/参院選2025.md
  - raw/external_brain_in_markdown/pages/参院選2025広聴AIふりかえり.md
  - raw/external_brain_in_markdown/pages/参院選2025 マニフェスト比較.md
- **entities**: 参院選, 広聴AI
- **tags**: ブロードリスニング, 選挙, 参院選, 2025
- **status**: confirmed
- **summary**: 参院選 2025 で広聴AI を用いた分析。マニフェスト比較・台湾からの声分析も実施。

### D106 再生の道ブロードリスニング
- **date**: 2025-04-25 〜 参院選2025
- **refs**:
  - raw/external_brain_in_markdown/pages/再生の道ブロードリスニング.md
  - https://news.ntv.co.jp/category/society/80d8b8a70586460bbc8894b2cc9a3994
- **entities**: 再生の道, 石丸伸二, 安野貴博, 広聴AI
- **tags**: ブロードリスニング, 政党, 参院選, 2025
- **status**: confirmed
- **summary**: 政党「再生の道」が参院選 2025 で活用予定とブロードリスニングを発表。安野氏が解説動画公開。

### D107 渋谷区ブロードリスニング
- **date**: 2025（令和7年度実施、令和6年度データ対象）
- **refs**:
  - raw/external_brain_in_markdown/pages/渋谷区ブロードリスニング.md
  - https://www.city.shibuya.tokyo.jp/kusei/kocho/questionnaire/kuminishikichosa_ai.html
- **entities**: 渋谷区, 区民意識調査
- **tags**: ブロードリスニング, 自治体, 2025
- **status**: needs-date
- **summary**: 渋谷区が区民意識調査の自由回答 6,037 件を対象に「ブロードリスニング」トライアル実施。具体的な実施月は要確認。

### D108 朝日新聞ブロードリスニング
- **date**: 2025-05-25（初出記事）
- **refs**:
  - raw/external_brain_in_markdown/pages/朝日新聞ブロードリスニング.md
  - https://www.asahi.com/articles/AST5Q3DZ4T5QUTFK001M.html
  - https://github.com/asahi-research/TTTC_consumption_tax_20250525
- **entities**: 朝日新聞, Talk to the City, Flourish
- **tags**: ブロードリスニング, メディア, 2025
- **status**: confirmed
- **summary**: 朝日新聞が消費税減税の投稿を AI 分析、散布図をニュース記事に埋め込み。参院選 2025 では X 投稿の AI 分析も実施。

### D109 企業内ブロードリスニング / サイボウズ社内事例
- **date**: 2024-09-10（初事例）
- **refs**:
  - raw/external_brain_in_markdown/pages/サイボウズ社内でのブロードリスニング活用事例.md
  - raw/external_brain_in_markdown/pages/企業内ブロードリスニング.md
- **entities**: サイボウズ, kintone, Talk to the City
- **tags**: ブロードリスニング, 企業, 内部事例, 2024
- **status**: confirmed
- **summary**: 100 人のマネージャー参加の企業文化 WS にブロードリスニング適用。15時データ → 17時レポートのタイトスケジュール。マス政治以外への応用の代表事例。

### D110 広聴AI 開発（DD2030）
- **date**: 2024 〜 ongoing
- **refs**:
  - raw/external_brain_in_markdown/pages/広聴AI.md
  - raw/external_brain_in_markdown/pages/広聴AI v3.0.md
  - raw/external_brain_in_markdown/pages/広聴AI開発定例:チームみらいの活動から見えてきたこと.md
- **entities**: デジタル民主主義2030, dd2030, Talk to the City
- **tags**: ブロードリスニング, ツール開発, ongoing
- **status**: ongoing
- **summary**: dd2030 の主力ツール。v3.0 までバージョンアップ。Cartographer / MindTrellis 等との比較設計も並走。

### D111 サステナブル・ブランド国際会議 2026 登壇
- **date**: 2026-02-19
- **refs**:
  - raw/external_brain_in_markdown/pages/サステナブル・ブランド国際会議 2026.md
  - https://sb-tokyo.com/2026/
- **entities**: 矢野和男, 矢島美代, 星賢人, 齋藤紘良, 山岡仁美, 権永詞
- **tags**: 登壇, 国際会議, Plurality, ウェルビーイング, 2026
- **status**: confirmed
- **summary**: 2 セッション登壇。「プルラリティで実装する真のウェルビーイング 〜分断社会の設計図」「Well-beingの新潮流」。ブロードリスニングを橋渡しの技術として議論。

### D112 DX&AI Forum 2024 登壇
- **date**: 2024
- **refs**:
  - raw/external_brain_in_markdown/pages/DX&AI Forum 2024 生成AIで作るデジタル民主主義の未来.md
- **entities**: DX&AI Forum
- **tags**: 登壇, 2024
- **status**: needs-date
- **summary**: 「生成AIで作るデジタル民主主義の未来」のセッション。具体日付要確認。

### D113 2026衆院選 ブロードリスニング
- **date**: 2026-02-07 〜 2026-02-08
- **refs**:
  - raw/external_brain_in_markdown/pages/2026衆院選最終日2026-02-07.md
  - raw/external_brain_in_markdown/pages/2026衆院選投票日2026-02-08.md
- **entities**: 衆院選
- **tags**: ブロードリスニング, 選挙, 衆院選, 2026
- **status**: confirmed
- **summary**: 2026 衆院選期間。具体的な関与内容は要本人確認。

---

## 3. 著書 / 執筆中

### D201 Jython プログラミング
- **date**: 2008
- **refs**: raw/external_brain_in_markdown/pages/自己紹介.md（初期 bio）
- **entities**: Jython
- **tags**: 著書, 2008, 在庫なし
- **status**: confirmed
- **summary**: Java で実装された Python 処理系 Jython の本。Java の硬さと Python の柔らかさの組み合わせ。

### D202 言語設計の基礎知識（WEB+DB PRESS Vol.60 特集）
- **date**: 2011
- **refs**: raw/external_brain_in_markdown/pages/自己紹介.md
- **entities**: WEB+DB PRESS
- **tags**: 寄稿, 特集, 2011
- **status**: confirmed
- **summary**: 言語の設計思想（何を目的として作られたか）を扱う特集。

### D203 コーディングを支える技術
- **date**: 2013-04-24
- **refs**:
  - http://nhiro.org/langbook/
  - https://www.amazon.cn/dp/B00M6KMQJU （中国語版）
- **entities**: 技術評論社
- **tags**: 著書, 2013, ロングセラー, 中韓翻訳
- **status**: confirmed
- **summary**: プログラミング言語進化を扱う技術書。中国語・韓国語翻訳。

### D204 word2vec による自然言語処理
- **date**: 2014-05
- **refs**: raw/external_brain_in_markdown/pages/自己紹介.md
- **entities**: word2vec, 技術評論社
- **tags**: 著書, 2014, 機械学習
- **status**: confirmed
- **summary**: word2vec 黎明期の解説書。本人の機械学習層活動の代表作。

### D205 世界一わかりやすいプログラミングのしくみ
- **date**: 2018
- **refs**: raw/external_brain_in_markdown/pages/自己紹介.md
- **entities**: 技術評論社
- **tags**: 著書, 2018, 入門書, 繁体字中国語翻訳
- **status**: confirmed
- **summary**: 入門書。繁体字中国語翻訳あり。

### D206 エンジニアの知的生産術
- **date**: 2018
- **refs**:
  - raw/external_brain_in_markdown/pages/エンジニアの知的生産術.md
  - 第5刷増刷ニュース（2024）
- **entities**: 技術評論社
- **tags**: 著書, 2018, ロングセラー, 第5刷
- **status**: confirmed
- **summary**: 知的生産技術書。2024 年に出版 5 年以上経過して増刷（ロングセラー化）。

### D207 PLURALITY 邦訳（サイボウズ式ブックス）
- **date**: 出版時期要確認
- **refs**:
  - raw/external_brain_in_markdown/pages/Plurality和訳.md
  - raw/external_brain_in_markdown/pages/サイボウズ式ブックス.md
  - https://scrapbox.io/plurality-japanese/初めに読んでね
- **entities**: Audrey Tang, Glen Weyl, サイボウズ式ブックス, ライツ社
- **tags**: 著書, 翻訳, Plurality, リーダー
- **status**: needs-date
- **summary**: 『PLURALITY 対立を創造に変える、協働テクノロジーと民主主義の未来』邦訳プロジェクトリーダー。出版時期/状態を本人確認要。

### D208 ⿻ 數位 Plurality（英語原書 Contributor & Editor）
- **date**: 2024
- **refs**: raw/external_brain_in_markdown/pages/Plurality本にEditingで載ってる.md
- **entities**: Audrey Tang, Glen Weyl
- **tags**: 著書, 寄稿, Plurality, 編集, 2024
- **status**: confirmed
- **summary**: 英語原書 Contributor & Editor として名前掲載。

### D209 ブロードリスニング本（執筆中）
- **date**: 2026-02 出版社ボール
- **refs**:
  - raw/external_brain_in_markdown/pages/ブロードリスニング本.md
  - 週記2026-02-09~2026-02-14（Audrey Tang メッセージ記載）
- **entities**: Audrey Tang, dd2030
- **tags**: 著書, 執筆中, ブロードリスニング
- **status**: in-progress
- **summary**: 2026-02 末締切で執筆中。Audrey Tang からのメッセージを収録。チームみらいだけでなく色々な党・自治体・民間企業の事例を扱う。

### D210 LENCHI / LLMを使いこなすエンジニアの知的生産術（執筆中）
- **date**: 2024-04 〜 ongoing
- **refs**:
  - raw/external_brain_in_markdown/pages/LENCHI_前書き.md
  - raw/external_brain_in_markdown/pages/LENCHI_第一章：『エンジニアの知的生産術』を問い直す.md
  - raw/external_brain_in_markdown/pages/LLMを使いこなすエンジニアの知的生産術(講演資料).md
- **entities**: Claude, GPT
- **tags**: 著書, 執筆中, LLM, 知的生産
- **status**: in-progress
- **summary**: Scrapbox 公開しながら執筆中。前書きは Claude 3 Opus との対話で生成された実例。

### D211 Engineer's way of creating knowledge（英語版書籍）
- **date**: 既存（出版年要確認）
- **refs**: raw/external_brain_in_markdown/pages/Engineer's way of creating knowledge.md
- **entities**: Lynda Gratton（参照, Section 7.2.4.2 Serial Mastery）
- **tags**: 著書, 英語, 翻訳
- **status**: needs-date
- **summary**: エンジニアの知的生産術 の英語版。Section 7.2.4.2 で Serial Mastery を引用。出版時期・経緯要確認。

---

## 4. 自作システム / ツール

### D301 Keichobot
- **date**: 2019 〜 ongoing (2023-03 GPT 統合)
- **refs**:
  - [[../projects/Keichobot.md|wiki: Keichobot]]
  - [[../../sources/Keichobot-search.md|source: Keichobot-search]]
- **entities**: Keicho, ChatGPT
- **tags**: ツール, チャットボット, 言語化
- **status**: ongoing
- **summary**: 自作チャットボット。「言語化フェーズ」担当。LLM 以前から同コンセプトを実装、2023-03 に GPT 統合。

### D302 Kozaneba
- **date**: 2021-08 〜 ongoing
- **refs**:
  - [[../projects/Kozaneba.md|wiki: Kozaneba]]
  - [[../../sources/Kozaneba-search.md|source: Kozaneba-search]]
- **entities**: KJ法
- **tags**: ツール, デジタルKJ法, 一次元化
- **status**: ongoing
- **summary**: 自作デジタル文房具。「一次元化フェーズ」担当。Keichobot との分業設計。

### D303 Scrapbox ChatGPT Connector
- **date**: 2023-03-09
- **refs**: raw/external_brain_in_markdown/pages/自分のScrapboxをChatGPTにつないだ.md
- **entities**: Scrapbox, ChatGPT, RAG
- **tags**: ツール, RAG, 2023
- **status**: confirmed
- **summary**: 個人 RAG の第一弾。Scrapbox の 2 万記事 = 書籍 60 冊分を ChatGPT につないだ。

### D304 倍速会議
- **date**: 2026-02 外部紹介（社内開発時期要確認）
- **refs**:
  - サイボウズ社内システム、2026-02-18 社内イベント、2026-02-19 サステナブル・ブランド国際会議で外部紹介
  - raw/external_brain_in_markdown/pages/AIと倍速会議.md
- **entities**: サイボウズ
- **tags**: ツール, 集合熟議, 社内システム
- **status**: needs-date
- **summary**: 社内開発の意見集約ツール。外部経営者からの相談に「まずはこれを試して」と紹介推奨。

### D305 主観的興味深さ推定システム
- **date**: 2025-10-30
- **refs**:
  - raw/external_brain_in_markdown/pages/主観的興味深さ推定システム.md
  - [[../concepts/AI協働の4パターン.md|wiki: AI協働の4パターン]]
- **entities**: GPT5, Gaussian Process Regression, UCB, MMR
- **tags**: ツール, 個人化, D-パターン
- **status**: in-progress
- **summary**: 抽出された知見の個人化提示システム。GP 回帰 + UCB + MMR。D パターン実装第一弾。

### D306 チャットから知見を引き出すシステム
- **date**: 2025-10-29
- **refs**: raw/external_brain_in_markdown/pages/チャットから知見を引き出すシステム.md
- **entities**: GPT5
- **tags**: ツール, 知見抽出, 2025
- **status**: in-progress
- **summary**: チャットログから 5 軸（One-step-Forward / Bridge / Actionability / Falsifiable / Experienced）で知見を抽出。

### D307 ConnectingDots システム（構想中）
- **date**: 2026-03-27 〜
- **refs**:
  - raw/external_brain_in_markdown/pages/ConnectingDotsシステム.md
  - [[../concepts/ConnectingDots.md|wiki: ConnectingDots]]
- **entities**: KarpathyのLLM Wiki, connecting-dots-design
- **tags**: 設計中, 構想, 自己紹介, 歴史
- **status**: in-progress
- **summary**: 事実×解釈分離設計の構想。自己紹介・Plurality 史を同じ仕組みで扱う Dot/Story/View 3層。

### D308 複数 LLM Wiki プロジェクト群
- **date**: 2026-04 〜 ongoing
- **refs**:
  - raw/external_brain_in_markdown/pages/日記2026-05-07.md
  - raw/external_brain_in_markdown/pages/複数のLLM_Wikiに共通のインプット.md
- **entities**: LENCHI Wiki, ブロリス Wiki, Karpathy Wiki, 注釈駆動Wiki, 盲点カードLLM Wiki, **本Wiki (llm-wiki-about-nishio)**
- **tags**: メタプロジェクト, ペルソナ, 2026
- **status**: ongoing
- **summary**: 複数の LLM Wiki を並走させる「wikis-as-personas」実験。共通入力に対して異なる切り出しを比較する手動 orchestrator パターン。

---

## 5. コミュニティ / イベント参加

### D401 villagepump 参加
- **date**: 2022 〜 ongoing
- **refs**:
  - https://scrapbox.io/villagepump/
  - [[../concepts/始める-広げる-繋げる.md|3軸フレームの原典発生場所]]
- **entities**: inajob, sta, yosider, mtane0412 等
- **tags**: コミュニティ, Scrapbox, ongoing
- **status**: ongoing
- **summary**: 共同編集 Scrapbox。「始める/広げる/繋げる」3軸フレームが生まれた場所。

### D402 LLM Meetup Tokyo #1 参加
- **date**: 2023-04-10
- **refs**: raw/external_brain_in_markdown/pages/2023-04-10 LLM Meetup.md
- **entities**: 安野貴博, LLM 無職
- **tags**: イベント, 2023
- **status**: confirmed
- **summary**: 全員 LLM 関連デモ持参の小規模ミートアップ。LLM 無職コミュニティが生まれた場。

### D403 Plurality Tokyo 系列
- **date**: 2023-2025
- **refs**:
  - raw/external_brain_in_markdown/pages/Plurality Tokyo.md
  - raw/external_brain_in_markdown/pages/Plurality Tokyo Keynote from Audrey Tang.md
- **entities**: Audrey Tang
- **tags**: イベント, Plurality, ongoing
- **status**: ongoing
- **summary**: Plurality Tokyo, Plurality Tokyo Salon, Plurality Tokyo Namerakaigi 等の主催/参加。

### D404 Plurality Summit 2024
- **date**: 2024
- **refs**: raw/external_brain_in_markdown/pages/Plurality Summit 2024.md
- **entities**: Audrey Tang, Glen Weyl
- **tags**: イベント, 国際, Plurality, 2024
- **status**: confirmed
- **summary**: Plurality Summit 2024 参加。

### D405 KJ法勉強会@ロフトワーク
- **date**: 要確認
- **refs**: raw/external_brain_in_markdown/pages/KJ法勉強会@ロフトワーク.md
- **entities**: ロフトワーク, Miro
- **tags**: イベント, KJ法
- **status**: needs-date
- **summary**: KJ法勉強会を実施。Miro 使用。「Kozaneba を作ったが、勉強会では Miro を使った」事例。

---

## 6. 寄稿 / 論文 / メディア記事

### D501 情報処理学会誌 2023 寄稿
- **date**: 2023-08
- **refs**:
  - raw/external_brain_in_markdown/pages/主観か客観かではなく、一人の主観から大勢の主観へ.md
- **entities**: 情報処理学会
- **tags**: 寄稿, 論文, 2023, あの図
- **status**: confirmed
- **summary**: 「主観か客観かではなく、一人の主観から大勢の主観へ」。ブロードリスニング解説で頻用される「あの図」の出典。CC0。

### D502 サイボウズ式 複業を始めた理由（2017）
- **date**: 2017
- **refs**: https://cybozushiki.cybozu.co.jp/articles/m001358.html
- **entities**: サイボウズ式, BeProud
- **tags**: メディア, 記事, 2017, 複業
- **status**: confirmed
- **summary**: 「たとえ報酬がゼロでも、複業をやっていた」サイボウズ・ラボを辞めずに機械学習の技術顧問を始めた理由。

### D503 サイボウズ式 R&D 組織論（2019）
- **date**: 2019
- **refs**: https://cybozushiki.cybozu.co.jp/articles/m005323.html
- **entities**: サイボウズ式
- **tags**: メディア, 記事, 2019, 組織論
- **status**: confirmed
- **summary**: 「マネジメントはいらない、論文数で評価しない──R&Dの理想を追求したサイボウズ・ラボ」。

### D504 サイボウズ式 Plurality 対談（2024）
- **date**: 2024
- **refs**: https://cybozushiki.cybozu.co.jp/articles/m006211.html
- **entities**: Audrey Tang, Glen Weyl, 関治之, サイボウズ式
- **tags**: メディア, 記事, Plurality, 2024
- **status**: confirmed
- **summary**: 「対立する意見を糧に、デジタル技術で世界の分断をつむぎなおす」Audrey Tang × Glen Weyl × Code for Japan 関治之 対談。

### D505 レバテックラボ「写経」論争フォーカス記事
- **date**: 要確認
- **refs**: https://levtech.jp/media/article/focus/detail_604/
- **entities**: レバテックラボ
- **tags**: メディア, 記事, 教育
- **status**: needs-date
- **summary**: 「『写経』論争と、教育者/学習者のすれ違いに潜むモノ。西尾泰和氏が語る "少しでもマシ" な教育法」。

### D506 ゆるコンピュータ科学ラジオ Polis 回 出演
- **date**: 要確認
- **refs**: raw/external_brain_in_markdown/pages/ゆるコンピュータ科学ラジオPolis回.md
- **entities**: ゆるコンピュータ科学ラジオ, Polis
- **tags**: メディア, ポッドキャスト, Polis
- **status**: needs-date
- **summary**: Polis を扱う回に出演。

---

## 7. 新しい思想的アウトプット (2025-2026)

### D601 AI協働の4パターン (A/B/C/D)
- **date**: 2025-10-29
- **refs**:
  - raw/external_brain_in_markdown/pages/思考の結節点2025-10-29.md
  - [[../concepts/AI協働の4パターン.md|wiki: AI協働の4パターン]]
- **entities**: ブロードリスニング, RAG, AI インタビュアー
- **tags**: 思想, 概念, 2025
- **status**: confirmed
- **summary**: A=要約 / B=RAG / C=AIインタビュアー / D=データ間結合発見。D が新提案。

### D602 自己紹介と歴史は共通の構造を持つ
- **date**: 2026-02-11
- **refs**:
  - raw/external_brain_in_markdown/pages/自己紹介と歴史は共通の構造を持つ.md
  - [[../concepts/自己紹介と歴史は共通の構造を持つ.md|wiki: 同概念]]
- **entities**: Sonar, GPT5, dd2030, g0v
- **tags**: 思想, 概念, Dot, Story, View, 2026
- **status**: confirmed
- **summary**: Dots/Stories/Views 3 層構造。個人と公共を同じシステムで扱える設計。**本ファイル自身がその実装の前段**。

### D603 シリアルマスタリー自己診断
- **date**: 2025-12-01
- **refs**:
  - raw/external_brain_in_markdown/pages/日記2025-12-01.md
  - [[../concepts/シリアルマスタリー.md|wiki: シリアルマスタリー]]
- **entities**: Lynda Gratton, Plurality, LLM 無職
- **tags**: 思想, 自己認識, 2025
- **status**: confirmed
- **summary**: 「Plurality に出会ってから今が修士1年であるかのように振る舞っている → これってシリアルマスタリーだな」と自己診断。

### D604 始める/広げる/繋げる の C>A>B プロファイル
- **date**: 2023-03-05
- **refs**:
  - raw/external_brain_in_markdown/pages/始める-広げる-繋げる.md
  - [[../concepts/始める-広げる-繋げる.md|wiki: 同概念]]
- **entities**: villagepump, inajob, sta
- **tags**: 思想, 自己認識, 2023
- **status**: confirmed
- **summary**: 3 軸自己評価フレーム。本人 C>A>B（C:繋げる > A:始める > B:広げる）、Bが低い=飽きっぽい。

### D605 戦略的曖昧化 / 辺縁が育てばそれが中心
- **date**: 2025-2026
- **refs**:
  - [[../concepts/戦略的曖昧化.md|wiki: 戦略的曖昧化]]
  - [[../concepts/辺縁が育てばそれが中心.md|wiki: 辺縁が育てばそれが中心]]
- **entities**: -
- **tags**: 思想, 概念, 2025, 2026
- **status**: confirmed
- **summary**: 不確実性活用のための意図的曖昧化と、重心移動の動的構造論。曖昧な停滞 の対概念。

### D606 N=1 でも重要な意見とは橋 / 気づき = 橋
- **date**: 2025-10-22
- **refs**: raw/external_brain_in_markdown/pages/N=1でも重要な意見とは橋かもしれない.md
- **entities**: ブリッジング, ブリッジングボーナス, 予期せぬ新結合
- **tags**: 思想, 概念, 2025
- **status**: confirmed
- **summary**: N=1 の重要意見 = 橋 = 予期せぬ新結合。D パターンの理論的基盤の一つ。

---

## 8. ペルソナ / 自己認識更新

### D701 「修士1年として振る舞う」
- **date**: 2025-12-01 自己診断
- **refs**: raw/external_brain_in_markdown/pages/今が修士1年であるかのように.md
- **entities**: Plurality
- **tags**: 自己認識, シリアルマスタリー, 2025
- **status**: confirmed
- **summary**: Plurality に出会って以降「今が修士1年であるかのように」振る舞う。きっかけは LLM無職、表現は「アラフォー社会人ムーブから修士課程学生ムーブに切り替えた」。

### D702 wikis-as-personas 実験
- **date**: 2026-05
- **refs**: raw/external_brain_in_markdown/pages/複数のLLM_Wikiに共通のインプット.md
- **entities**: LENCHI, ブロリス本Wiki, Karpathy Wiki, **本Wiki**, MindTrellis
- **tags**: 自己認識, メタプロジェクト, 2026
- **status**: ongoing
- **summary**: 複数 Wiki を並走させ仮想人格として比較する実験。MindTrellis を 3 Wiki に投げて差分を比較した実例あり。

---

## 9. 学歴 / 経歴（基礎カード、参考まで）

### D801 博士（理学）取得
- **date**: 2006（24歳）
- **refs**: raw/external_brain_in_markdown/pages/自己紹介.md
- **entities**: NAIST
- **tags**: 学歴
- **status**: confirmed
- **summary**: 24歳で博士（理学）取得。京大情報学科 → NAIST 博士前期飛び級 → 短期修了 2 回。

### D802 技術経営修士取得
- **date**: 2014
- **refs**: raw/external_brain_in_markdown/pages/自己紹介.md
- **entities**: 東京工業大学
- **tags**: 学歴
- **status**: confirmed
- **summary**: 会社員の傍ら東工大で取得。

### D803 サイボウズ・ラボ 主幹研究員
- **date**: 2007 〜 ongoing
- **refs**: raw/external_brain_in_markdown/pages/自己紹介.md
- **entities**: サイボウズ・ラボ
- **tags**: 役職, 本職
- **status**: ongoing
- **summary**: 2007 年入社。チームワークや知的生産性を高めるソフトウェアの研究。主幹研究員。

### D804 2002年度未踏スーパークリエータ
- **date**: 2002
- **refs**: raw/external_brain_in_markdown/pages/自己紹介.md（"双方向通信型３Ｄワールドシミュレーター"）
- **entities**: IPA, 未踏ユース, 3D-NWS, アントラッド
- **tags**: 受賞, 未踏, 2002
- **status**: confirmed
- **summary**: 初年度の未踏ユース採択（20歳）。3D 仮想空間でエージェント環境相互作用や遺伝的アルゴリズムを実装。

### D805 未踏ジュニア コファウンダー・メンター
- **date**: 2016 〜 ongoing
- **refs**:
  - https://jr.mitou.org/
  - raw/external_brain_in_markdown/pages/未踏ジュニア.md
- **entities**: 一般社団法人未踏, 未踏ジュニア
- **tags**: 役職, 未踏ジュニア, ongoing
- **status**: ongoing
- **summary**: 17 歳以下のクリエータ支援プログラムのコファウンダー兼メンター。継続中。

### D806 BeProud 機械学習関連の技術顧問
- **date**: 2017 〜 状態要確認
- **refs**: raw/external_brain_in_markdown/pages/自己紹介.md
- **entities**: BeProud
- **tags**: 役職, 兼務, 2017
- **status**: needs-date
- **summary**: 機械学習関連の技術顧問。現在も継続中か要本人確認。

---

## 統計

- 合計: 47 Dot
- status 別:
  - confirmed: 33
  - ongoing: 8
  - in-progress: 5
  - needs-date: 9（重複あり）
- カテゴリ別:
  - 役職: 6 (D001-D006)
  - ブロードリスニング案件: 13 (D101-D113)
  - 著書: 11 (D201-D211)
  - 自作システム: 8 (D301-D308)
  - コミュニティ: 5 (D401-D405)
  - 寄稿/メディア: 6 (D501-D506)
  - 思想: 6 (D601-D606)
  - 自己認識: 2 (D701-D702)
  - 学歴/経歴: 6 (D801-D806)

## 次の運用

1. 本人レビュー → 各 Dot に対し ✅ / ❌ / 修正 / 不要 をマーク
2. ✅ Dot を JSON 化（自動変換可能）して entrypoint リポジトリに import
3. needs-date / needs-verification Dot は本人補完または別途調査
4. Story 編集時、本ファイルから ID で参照（D101 / D207 等）して並べる

## 関連

- [[../syntheses/欠落Dot-2026.md|欠落Dot-2026]] — 本ファイルの基となった欠落調査
- [[../meta/目的-自己紹介ページ更新.md|目的-自己紹介ページ更新]] — 第一目的方針
- [[../concepts/自己紹介と歴史は共通の構造を持つ.md|自己紹介と歴史は共通の構造を持つ]] — Dot/Story/View 3層論
- [[../concepts/自己紹介ポーカー.md|自己紹介ポーカー]] — 役を作る理論
- [[../../sources/自己紹介-bios.md|自己紹介-bios]] — 既存 bio 履歴

## Open Questions

- **D207 Plurality 邦訳本**の出版状況（出版済 / 予定 / 取り止め）が外部脳から判定できない、要本人確認
- **D304 倍速会議**の開発開始時期不明（2026-02 外部紹介は確実）
- **D211 Engineer's way of creating knowledge** の出版経緯（翻訳 or 並行執筆 or 部分公開）
- **D107 渋谷区 / D112 DX&AI Forum / D405 KJ法勉強会 / D505 レバテックラボ / D506 ゆるコンピュータ科学ラジオ**の具体日付
- 「**未踏ジュニア で何件メンターしたか**」を集約 Dot とするか、個別案件を Dot 化するか
- 守秘契約等で bio に出せない案件がある場合、本ファイルに status: confidential のような区別を追加するか
- Dot ID 体系（カテゴリ番号 + 連番）を続けるか、Scrapbox の page ID 的なハッシュにするか
