---
type: project
summary: nishio自作のデジタル文房具。2021-08起動、現在進行形。知的生産プロセスの「一次元化フェーズ」を担う
sources:
  - Kozaneba-search.md
  - raw/external_brain_in_markdown/pages/Kozaneba.md
  - raw/external_brain_in_markdown/pages/Keichobotは言語化しKozanebaは一次元化する.md
---

# Kozaneba

nishio自作のデジタル文房具。"a digital stationary to organize your thought"。
公開URL: [https://kozaneba.netlify.app/](https://kozaneba.netlify.app/)

## 役割

[[Keichobot.md|Keichobot]] とペアで知的生産プロセスを構成：

- Keichobot = **言語化**（モヤモヤ→シンボル→関係）
- Kozaneba = **一次元化**（関係を客体化→ストーリーへ並べる）

→ Kozaneba は「**すでに言語化されたものを構造化・物語化する**」段階の専用ツール。
  - こざね一枚一枚の中身は言語化済みで、配置の近さはまだ言語化されていない。lenchi や kozaneba-dev-ai が Kozaneba を「前言語的な構造化に強い」と書くのは、この配置の側を指している。

## KJ法系譜の中での位置

[[../../sources/KJ法-search.md|KJ法系譜]] において：

- 物理KJ法（1960s）: 「近接配置」で関係を表現
- Kozaneba: 「**線**」で関係を明示 → **既存の構造を保ったまま別の構造化が可能** に
- 詳細: [Keichobotは言語化しKozanebaは一次元化する.md](../../raw/external_brain_in_markdown/pages/Keichobotは言語化しKozanebaは一次元化する.md) "なぜ線が必要不可欠か"

## 開発の波

- **2021-08** 起動（前身 Movidea から）、集中開発期
- **2022-2023** 断続的開発
- **2025** pKozaneba 連続更新で再活発化（pKozaneba2025-03-11 / 08-14 / 08-26~27 / 08-29 / 09-11）

## Kozaneba: プレフィックスの活用

`Kozaneba:` を冠したページ群は **Kozaneba 上で整理した結果のスナップショット**。対象は多様：

- 哲学: 体験過程と意味の創造（ジェンドリン）/ 言語の現象学について / コンヴィヴィアリティ（イリイチ）
- 宗教思想: 華厳経 / 荘子
- 自己研究: この10年のプログラミング言語の変化 / Scrapboxベストプラクティス2022 / ねりねり

→ **思想の整理場として継続的に使われている**。

## 自己再帰的な使い方

- Kozanebaの開発をKozanebaで管理
- Kozanebaのコードを丸ごとo1 Proに入れる
- LENCHI_Day1時点のKozaneba / Day3時点のKozaneba — LLM時代の知的生産術本の執筆素材として

## エコシステム

- Scrapbox連携: Kozaneba+Scrapbox / Scrapboxの行とKozanebaのこざねの対応づけ / Scrapboxプロジェクトをインポート
- [/kozaneba-forum/Kozaneba](https://scrapbox.io/kozaneba-forum/Kozaneba) — フォーラムあり
- 探検ネット勉強会Kozaneba 1〜5 — 勉強会シリーズ

## 停滞している意思決定

- **Kozanebaの次の進む方向についてわかると良い**（2021-09-01）— [[../concepts/曖昧な停滞.md|曖昧な停滞]] の当時の事例。2026-05-16 に Plan B（現行改造）と Plan A（新規）の並行で決着（kozaneba-dev-ai）
- Kozanebaにエッジラベルをつけると良いのでは — 仕様の保留
- TwitterをKozanebaに入れたい — 機能追加案の保留

→ 開発継続中だが「次の方向」が複数並走している典型パターン。

## 関連

- [[Keichobot.md|Keichobot]] — ペア
- [[../../sources/KJ法-search.md|KJ法系譜]]
- [[../concepts/ConnectingDots.md|ConnectingDots]] — Dot粒度設計でKozanebaのこざねは1つのDot候補
- [[../topics/知的生産.md|知的生産]]

## Open Questions

詳細サーベイの Open Questions は [[../../sources/Kozaneba-search.md|Kozaneba-search]] 参照。 2026-11-07の現状照合による解決・前提変更は、参照先を上書きせず本ページの Updates に追記した。

- 「Kozanebaの次の進む方向についてわかると良い」の意思決定保留はいつから続いているか

## Updates

- 2026-11-07: 参照先のOpen Questionsの現状を補足 — 参照先 `sources/Kozaneba-search.md` の「2025年の pKozaneba 急増は何が引き金か（外的要求？個人的再注力？）」。2025-08のCanvas実験には広聴AIのデータ配置との接続が原文にある。2025年全体の増加を一つの原因で説明する証拠ではない。（根拠: 公開 Cosense の原記録（2025-08-26〜27）、`/Users/nishio/kozaneba-dev-ai/raw/scrapbox_kozaneba/2025-08-26__pKozaneba2025-08-26~27.md:28`；kozaneba-dev-ai 2026-05-19 git履歴調査のLOG、`/Users/nishio/kozaneba-dev-ai/wiki/log.md:227`）
- 2026-11-07: 参照先のOpen Questionsの現状を更新 — 参照先 `sources/Kozaneba-search.md` の「「Kozanebaの次の進む方向についてわかると良い」の意思決定保留はいつから続いているか」。元メモの作成日は2021-09-01、2026-05-16のLOGにはPlan BとPlan Aの並行方針が記録されている。Codex の検証（2026-11-07）で「閉じる」から戻した: 作成日は保留が連続している期間を示さず、2021年の機能選択と2026年の改造・新規並行方針は同じ問いとは確認できない。後続の2026-06の追記にはPlan Aの判断は引き続き保留とある。（根拠: 6f80d87・2026-09-30 23:59 LOG、`log.md:332`；`/Users/nishio/kozaneba-dev-ai/raw/scrapbox_kozaneba/2021-09-01__Kozanebaの次の進む方向についてわかると良い.md:3`；2026-05-16 LOG、`/Users/nishio/kozaneba-dev-ai/wiki/log.md:212`；`/Users/nishio/kozaneba-dev-ai/wiki/themes/3plan議論.md:145`）
- 2026-11-07: 参照先のOpen Questionsの現状を補足 — 参照先 `sources/Kozaneba-search.md` の「Kozaneba と ConnectingDots は同じツール系譜の別ブランドか、別物か」。同じ別ブランドと断定する根拠はなく、ConnectingDotsには独立した実装がある。接続が未着手であることまで更新する。（根拠: connecting_dots 579bd66（2026-08-01）、`/Users/nishio/connecting_dots/HANDOFF.md:9`・`/Users/nishio/connecting_dots/HANDOFF.md:84`；29aa9ca・2026-10-07 の実装照合記録、`/Users/nishio/connecting-dot-design/wiki/open-questions.md:234`）
