# GitHub Profile README 要件定義

## 1. 目的

GitHubプロフィールを、装飾中心の自己紹介から、採用担当者・開発責任者・Founderが20〜30秒で以下を判断できる「受託用の技術プロフィール」へ再設計する。

- 誰で、どのようなエンジニアか
- 何を依頼できるか
- どのような成果を出したか
- 技術と担当範囲を裏付ける公開コードがあるか
- 現在相談可能か、どこから連絡できるか

## 2. 想定読者

1. フリーランス / 業務委託エンジニアを探す採用担当者・EM・CTO
2. 0→1開発、PoC、AI自動化、Solana連携を依頼したいFounder / PM
3. 公開リポジトリや技術判断を確認したいエンジニア・OSS contributor
4. 日本語話者を主対象としつつ、海外チーム・英語話者にも同じ情報を提供する

## 3. 情報源と事実確認方針

### 提供資料（非公開）

- 2026-08-20時点の日本語職務経歴書
- 日本語スキルマトリクス
- 英語レジュメ

### 公開証拠

- [Axis MVP](https://github.com/Axis-pizza/Axis_MVP)
- [Axis AMM](https://github.com/Axis-pizza/Axis_AMM)
- [ctsDAO Landing Page](https://github.com/muse0509/ctsdao_lp)
- [Axis MCP](https://github.com/Axis-pizza/Axis_mcp)
- `muse0509`が作成した公開Pull Requestとcommit履歴

### 表現ルール

- 資料間で数値が異なるAxis実績は、保守的な丸め値「約400ユーザー / 2,100件超」を使う
- Axisの利用実績には必ず`Devnet`と明記し、Mainnetの売上・TVLと誤認させない
- クライアント案件は、公開許可が確認できない実装詳細・コード・内部構成を載せない
- Rust / Pinocchioは主力言語と断定せず、公開リポジトリで確認できる`Program R&D / testing`の文脈で示す
- 英語力は資格ではなく、技術MTG・要件調整・交渉・ピッチの対応経験として示す
- 年齢、性別、住所、電話番号は掲載しない

## 4. 調査したベストプラクティス

調査日: 2026-08-26

| Source | 採用する示唆 |
| --- | --- |
| [GitHub Docs — Managing your profile README](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme) | ユーザー名と同名のpublic repository、rootの`README.md`を日本語の既定表示にする |
| [GitHub Docs — Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#relative-links) | 日英READMEの相互移動にはbranchに追従するrelative linkを使う |
| [Qiita — 5分でできる！GitHub README プロフィール](https://qiita.com/mmnn/items/cf465d271171cba8bd51) | シンプルさを保ち、スキルと活動を短時間で把握できる構成にする |
| [Qiita — 未経験者が自社開発企業に就職するためのREADME書き方](https://qiita.com/teruis/items/64fcf585f02162fa2f3b) | 発注者がコードを細部まで読まない前提で、端的・視覚的に概要、技術、強みを伝える |
| [Zenn — 読みたくなるREADMEを書くためのコツ](https://zenn.dev/bloomer/articles/3f73f7d02e5a63) | 読み手が知りたい順に、一言、視覚、URL、概要、技術を配置する |
| [Zenn — README.md 日本語と英語の切り替えボタンの実装](https://zenn.dev/keitosuwahara/articles/2529e2685773ed) | `README.md`と別言語ファイルを相対リンクで相互遷移させる |
| [Qiita — GitHubプロフィールREADMEを、オリジナルカードを追加する方法](https://qiita.com/0ts_st/items/c58dcefade70f0c4a024) | Profile READMEを第一印象を作る案内板として設計し、静的カードで世界観を伝える |
| [Zenn — GitHubのプロフィールREADMEを作ってみた](https://zenn.dev/uya0526_design/articles/zenn_github-profile-readme) | 実務経験と学習中を分け、projectに技術・役割・証拠を付ける。外部Stats障害を重要導線に持ち込まない |
| [Zenn — GitHub Actionsで安定したプロフィールREADMEを錬成してみた](https://zenn.dev/toramutton/articles/eb21f46932fd34) | 第三者の動的画像は表示不安定性と運用負荷があるため、Heroをrepository内の静的SVGにする |
| [フリーランスエンジニアのGitHubアピール術](https://syusodo.co.jp/workee-freelance-blog/articles/freelance-engineer-github-for-jobs) | 一行自己紹介、直近実績、対応領域、稼働状況、連絡導線、NDA配慮を明示する |

## 5. 機能要件

| ID | 要件 |
| --- | --- |
| FR-01 | `README.md`を日本語のprofile defaultとして表示する |
| FR-02 | `README.en.md`に同一構造・同一事実の英語版を用意する |
| FR-03 | 各READMEの最上部に日本語 / Englishの切り替え導線を置く |
| FR-04 | First viewに氏名、肩書き、専門領域、案件相談CTA、主要連絡先を置く |
| FR-05 | 約400 Devnet users、2,100+ baskets、400+ leads、5-person teamを一目で比較できる形にする |
| FR-06 | 対応領域を発注単位で表現し、単なるtechnology badge一覧にしない |
| FR-07 | Selected Workは役割、担当、成果、stack、evidence linkを同じ順序で示す |
| FR-08 | Public workとNDA対象のclient workを明確に分ける |
| FR-09 | 技術stackはArea、technology、実務用途の3列で示す |
| FR-10 | Email、LinkedIn、X、Portfolioへのcontact routeを上部と末尾に置く |

## 6. 情報設計

1. Language switch
2. Static hero
3. Name / positioning / primary links / availability CTA
4. Quantified impact
5. Profile summary
6. What I can help with
7. Selected public work
8. Client work and NDA note
9. Core stack with production context
10. How I work
11. Writing and recognition
12. Contact CTA

## 7. ビジュアル要件

- Tone: `dark editorial / quiet luxury`
- Palette: Cinema Void `#020201`、warm ivory `#F6F0E7`、rose bronze `#C77D36`
- Repository内の静的SVGを使用し、Heroの表示を外部サービスに依存させない
- アニメーション、巨大ASCII art、大量のbadge / logo、trophy / snake / 3D graphを主要導線に使わない
- 高級感を「少ない色、余白、整列、明確なhierarchy、定量証拠」で作る
- GitHubが許可しないcustom CSSやJavaScriptを前提にしない
- Heroとlanguage buttonにalt / titleを付ける
- 1200px幅のHeroを`width="100%"`で表示し、mobileでも縮小可能にする

## 8. 日英切り替え仕様

GitHub Profile READMEはsanitized static Markdownであり、JavaScriptによるin-place tab switchingやbrowser language detectionは実装できない。

- Japanese: `README.md`
- English: `README.en.md`
- 表示方法: repository内の静的SVG button + relative link
- 日本語をdefault表示とし、英語版は1 clickで開く
- 2ファイルのsection順、metrics、linksを同期する

## 9. 非機能要件

- 外部のdynamic image APIが停止しても、氏名、肩書き、実績、contactが失われない
- 公開情報のみで構成し、credentials、private repository、client sourceを含めない
- Markdown / SVGはGitHubで安全にrenderできるsyntaxに限定する
- 主要relative linkとasset pathが存在する
- 日本語・英語で数値、role、project順、contactに不一致がない
- README本文は発注者がskimmingできる見出しと短い段落を基本とする

## 10. 受入条件

- [ ] `README.md`が日本語で始まり、GitHub profileに表示できる
- [ ] `README.en.md`との相互linkが機能する
- [ ] First viewだけで「誰 / 何ができる / 相談可能 / contact」が分かる
- [ ] Skillは用途つきで分類され、実績にはrole・impact・evidenceがある
- [ ] Axis数値にDevnet表記があり、research repositoryにunaudited表記がある
- [ ] Client workにNDA配慮がある
- [ ] 全SVGがwell-formedで、light / dark themeの両方で読める固定dark cardとして表示される
- [ ] 全local link / image pathが存在する
- [ ] 外部URLの表記とmailtoが正しい
- [ ] 日本語・英語のclaimsが同期している

## 11. 運用

- 稼働状況と日付は月1回、またはavailability変更時に更新する
- 実績数値はsourceとenvironment（Devnet / Mainnet）を確認してから更新する
- Projectを追加する場合は`Role / Work / Impact / Stack / Evidence`を揃える
- 日本語・英語を同一Pull Requestで更新する
- ProfileのPinned repositoriesは、READMEのSelected Workと合わせて定期的に見直す
