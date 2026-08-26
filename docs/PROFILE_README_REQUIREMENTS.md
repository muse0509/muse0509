# GitHub Profile README 要件定義

更新日: 2026-08-26  
方針: Skills-first / Single README

## 1. 目的

GitHubプロフィールを、作品や成果を並べるポートフォリオではなく、採用担当者・開発責任者・Founderが短時間で「この技術者に何を依頼できるか」を判断できる受託用プロフィールにする。

- TypeScriptを軸としたFull-stack開発力を最初に伝える
- AI / RAG・業務自動化、Solana / Web3、Technical Leadの対応範囲を示す
- 日本語話者と英語話者に同じ情報を一つのページで提供する
- 稼働条件と問い合わせ先を迷わず確認できるようにする

## 2. 想定読者

1. フリーランス / 業務委託エンジニアを探す採用担当者・EM・CTO
2. 0→1開発、MVP、AI自動化、Solana連携を依頼したいFounder / PM
3. 技術領域と公開コードを確認したいエンジニア
4. 日本語話者を主対象としつつ、海外チーム・英語話者も対象とする

## 3. 今回の編集方針

前版のHero画像、言語切り替え画像、定量実績中心の構成は廃止する。

| 項目 | 採用する仕様 |
| --- | --- |
| 言語 | 一つの`README.md`に日本語、その下に英語を掲載 |
| First view | 氏名、肩書き、主要リンク、技術バッジ |
| 主役 | 「できること」と技術スタック |
| 実績 | 数値や受賞歴を強調せず、公開物を補助的な根拠として短く掲載 |
| 見た目 | 画像を作らず、余白・短い文章・統一したflat-square badgeで落ち着かせる |
| CTA | 日英それぞれに稼働条件とEmail / LinkedInを掲載 |

## 4. 情報源と表現ルール

### 提供資料

- 2026-08-20時点の日本語職務経歴書
- 日本語スキルシート
- 英語レジュメ

### 公開証拠

- [Axis MVP](https://github.com/Axis-pizza/Axis_MVP)
- [Axis AMM](https://github.com/Axis-pizza/Axis_AMM)
- [ctsDAO Landing Page](https://github.com/muse0509/ctsdao_lp)
- [Zenn](https://zenn.dev/yusukekikuta)

### 表現ルール

- 資料と公開情報で確認できる技術・担当範囲だけを記載する
- クライアント案件の非公開情報、private repository、個人情報を載せない
- Rust / Pinocchioは主力スキルのバッジにせず、公開物のProtocol R&Dとして扱う
- 英語力は資格ではなく、技術調整への対応力として示す
- 年齢、性別、住所、電話番号は掲載しない

## 5. 参考にしたベストプラクティス

| Source | 採用する示唆 |
| --- | --- |
| [GitHub Docs — Managing your profile README](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme) | ユーザー名と同名のpublic repositoryのrootに`README.md`を置く |
| [GitHub Docs — Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) | GitHub標準Markdownだけで、読みやすく保守しやすい構造にする |
| [Qiita — 5分でできる！GitHub README プロフィール](https://qiita.com/mmnn/items/cf465d271171cba8bd51) | スキルと活動を短時間で把握できるシンプルな構成にする |
| [Qiita — 未経験者が自社開発企業に就職するためのREADME書き方](https://qiita.com/teruis/items/64fcf585f02162fa2f3b) | コードを細部まで読まない読者にも概要、技術、強みを端的に伝える |
| [Zenn — 読みたくなるREADMEを書くためのコツ](https://zenn.dev/bloomer/articles/3f73f7d02e5a63) | 読み手が知りたい順に、一言、URL、概要、技術を配置する |
| [Zenn — GitHubのプロフィールREADMEを作ってみた](https://zenn.dev/uya0526_design/articles/zenn_github-profile-readme) | 技術領域を整理し、公開projectを根拠として添える |

## 6. 機能要件

| ID | 要件 |
| --- | --- |
| FR-01 | rootの`README.md`だけで日英両方を読める |
| FR-02 | 日本語を先に、区切り線の後に英語を掲載する |
| FR-03 | 最上部に氏名、肩書き、主要リンク、技術バッジを置く |
| FR-04 | バッジは主力技術に限定し、`flat-square`で統一する |
| FR-05 | 対応領域をFull-stack、0→1 / MVP、AI / RAG、自動化、Solana、Technical Leadに整理する |
| FR-06 | 技術スタックをFrontend、Backend / Data、AI / Automation、Solana / Web3、Cloud / Deliveryに分類する |
| FR-07 | 公開物は技術力の根拠として3件程度を短く掲載する |
| FR-08 | 稼働条件とEmail / LinkedInを日英それぞれに置く |
| FR-09 | Hero、言語切り替え画像、local SVG asset、別言語READMEを使用しない |
| FR-10 | 定量実績、受賞歴、長いproject case studyを主要コンテンツにしない |

## 7. 情報設計

1. 氏名 / 英字名
2. Positioning
3. Portfolio / Zenn / LinkedIn / X / Email
4. 技術バッジ
5. 日本語: 概要 / 稼働条件 / できること / 技術スタック / 公開物 / Contact
6. 区切り線
7. English: Overview / Availability / Capabilities / Stack / Public Work / Contact

## 8. ビジュアル要件

- custom Hero、生成画像、言語切り替え画像を使わない
- custom CSS、JavaScript、animationを前提にしない
- 技術バッジはShields.ioの`flat-square`で統一する
- GitHubのlight / dark themeの両方で本文が読める標準Markdownを使う
- 高級感は装飾ではなく、情報量の抑制、余白、見出しの階層、表記の統一で作る

## 9. 受入条件

- [ ] `README.md`が日本語から始まり、その下に英語版がある
- [ ] `README.en.md`とcustom SVG assetが存在しない
- [ ] First viewで肩書き、主要技術、主要リンクを確認できる
- [ ] 主力技術が統一されたバッジで表示される
- [ ] 「できること」が日英で対応し、担当可能範囲を把握できる
- [ ] 実績数値、受賞歴、長いcase studyが前面に出ていない
- [ ] 公開物へのlinkが技術力の補助的な根拠として機能する
- [ ] 稼働条件と問い合わせ先が日英で確認できる
- [ ] local image参照や存在しないrelative linkがない
- [ ] MarkdownがGitHub Flavored Markdownとしてparseできる

## 10. 運用

- 稼働条件が変わった場合は日本語・英語を同時に更新する
- 主力技術が変わった場合だけbadgeとstack分類を見直す
- 公開物は代表的な3件程度に絞り、増やしすぎない
- 画像制作や複雑な自動生成処理を追加せず、README単体で保守する
