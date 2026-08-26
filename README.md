<p align="right">
  <a href="./README.md"><img src="./assets/lang-ja-active.svg" alt="日本語" height="30" /></a>
  <a href="./README.en.md"><img src="./assets/lang-en.svg" alt="English" height="30" /></a>
</p>

<p align="center">
  <img src="./assets/profile-hero.svg" alt="Yusuke Kikuta - Full-stack Product Engineer" width="100%" />
</p>

<h1 align="center">菊田 佑輔 <sub>(Muse)</sub></h1>

<p align="center">
  <strong>TypeScriptを軸に、曖昧なアイデアを動くプロダクトへ変えるフルスタックエンジニア</strong>
</p>

<p align="center">
  <a href="https://yusuke-portfolio.yusukekikuta-05.workers.dev">Portfolio</a>
  &nbsp;·&nbsp;
  <a href="https://axs.pizza/">Axis</a>
  &nbsp;·&nbsp;
  <a href="https://zenn.dev/yusukekikuta">Zenn</a>
  &nbsp;·&nbsp;
  <a href="https://www.linkedin.com/in/yusukekikuta">LinkedIn</a>
  &nbsp;·&nbsp;
  <a href="https://x.com/muse_jp_sol">X</a>
  &nbsp;·&nbsp;
  <a href="mailto:yusukekikuta.05@gmail.com">Email</a>
</p>

> **業務委託のご相談を受付中です。** 2026年8月現在、週15〜20時間程度・フルリモートで参画可能です。0→1開発、PoC、技術リード、AI/RAG自動化、Solana連携のご相談は [Email](mailto:yusukekikuta.05@gmail.com) または [LinkedIn](https://www.linkedin.com/in/yusukekikuta) へご連絡ください。

## 実績ハイライト

|  |  |
| :---: | :---: |
| **約400**<br>Axis Devnetユーザー | **2,100+**<br>ユーザー作成バスケット |
| **400+**<br>リード獲得に貢献 | **5名**<br>プロダクト開発チーム |

Axisの数値はDevnet上の実績です。有償広告やユーザーインセンティブに依存せず獲得しました。

## Profile

TypeScript / Reactを中心に、Frontend、Backend、API、DB、AI自動化、Solana連携まで横断して開発しています。事業目的とユーザー体験から要件と優先順位を整理し、設計・実装・レビュー・リリース後の改善まで一気通貫で担当できることが強みです。

[Axis](https://axs.pizza/)ではTechnical Founder / Full-stack Engineerとして5名チームの開発を推進し、主要なFrontend・Backend実装、仕様調整、Pull Requestレビュー、リリース判断を担当しました。英語での技術ミーティング、要件調整、交渉、ピッチにも対応できます。

## 対応できること

| 領域 | 提供できる価値 |
| --- | --- |
| **0→1プロダクト開発** | 曖昧な要望の整理、MVPスコープ策定、技術選定、画面・API・DB設計、実装、リリース |
| **Full-stack Web** | React / Next.jsのFrontendから、Hono / Cloudflare WorkersのAPI・DB・運用まで一気通貫で開発 |
| **AI / RAG・業務自動化** | OpenAI API、RAG、Seleniumを用いた業務アプリ、AIエージェント、ブラウザ自動化の設計・実装 |
| **Solana / Web3** | Wallet接続、Transaction構築・署名、SPL Token、オンチェーン状態連携、DeFi UX、Program R&D・テスト |
| **Technical Lead** | 要件・設計レビュー、Pull Requestレビュー、品質・優先順位・リリース判断、海外チームとの技術調整 |

## Selected Work

### Axis — オンチェーン・バスケット型DeFiプロダクト

- **Role:** Technical Founder / Full-stack Engineer
- **Contribution:** 個人プロジェクトとして立ち上げ、初期Devnet PoCの主要Frontend / Backendを構築。React / ViteのSPA、Hono / Cloudflare Workers / D1のAPI・DB、Wallet接続、Transaction構築、分析・運用基盤を横断して開発し、その後は5名チームの仕様調整、レビュー、リリース判断を担当
- **Outcome:** Devnetで約400ユーザー・2,100件超のユーザー作成バスケットを獲得
- **Stack:** TypeScript, React, Vite, Tailwind CSS, Hono, Cloudflare Workers, D1, Drizzle ORM, Solana Web3.js
- **Evidence:** [Product](https://axs.pizza/) · [Repository](https://github.com/Axis-pizza/Axis_MVP) · [Dynamic OGP PR #117](https://github.com/Axis-pizza/Axis_MVP/pull/117) · [Edge cache PR #120](https://github.com/Axis-pizza/Axis_MVP/pull/120) · [Technical article](https://zenn.dev/yusukekikuta/articles/04904b02dcadfb)

### ctsDAO — Landing Page & Intake System

- **Role:** Full-stack Engineer
- **Contribution:** エディトリアルデザインのLanding Page、Zodによるフォーム検証、rate limiting、UTM / referral attribution、GA4 / PostHog、管理用JSON / CSV API、SQLite / PostgreSQLアダプターを実装
- **Outcome:** 問い合わせ受付、流入計測、管理用exportを一つの運用経路に統合
- **Stack:** Next.js App Router, TypeScript, Tailwind CSS, Zod, SQLite, PostgreSQL, GA4, PostHog
- **Evidence:** [Repository](https://github.com/muse0509/ctsdao_lp) · [Implementation PR #3](https://github.com/muse0509/ctsdao_lp/pull/3)

### Axis AMM — Solana Batch Auction Research

- **Role:** Product Lead / Protocol R&D
- **Contribution:** LVRを抑制するPeriodic Batch Auctionの要件、経済設計、検証条件、セキュリティ境界を定義し、コントラクトエンジニアと実装・テストを推進
- **Outcome:** 公開Project benchmarkで、注文数に依存しないO(1) ClearBatchをmedian 38,120 CU / p95 38,500 CUと計測
- **Stack:** Rust, Pinocchio, Solana, LiteSVM / local validator, Jito, Switchboard
- **Evidence:** [Research repository](https://github.com/Axis-pizza/Axis_AMM) — research software / unaudited prototype

## クライアントワーク・開発支援

- **AI営業自動化:** Python / OpenAI API / RAG / Selenium / AWSで、企業調査から営業文面生成、問い合わせフォーム送信、例外処理・再試行までを自動化。実運用で400件以上のリード獲得に貢献
- **生成AI・RAG業務アプリ:** AIへの入力、回答・参照情報、loading / error stateを含むReact FrontendとAPI連携を実装
- **Web3 MVP Mentoring:** Fracton Venturesで複数チームの要件整理、MVPスコープ、技術選定、コードレビューを支援し、Demo Dayまでの開発を推進

クライアントの守秘義務と契約条件に配慮し、ソースコードおよび詳細仕様は公開していません。公開可能な範囲の詳細は面談時に共有します。

## Core Stack

| Area | Technologies | 実務・開発での主な用途 |
| --- | --- | --- |
| **Frontend** | TypeScript, JavaScript, React, Next.js, Vite, Tailwind CSS | SPA、業務Webアプリ、非同期UI、レスポンシブUI、PWA |
| **Backend / Data** | Hono, Node.js, REST API, Cloudflare Workers, D1 / SQLite, PostgreSQL, Drizzle ORM, SQL | API・DB設計、migration、定期処理、data indexing、運用 |
| **AI / Automation** | Python, OpenAI API, RAG, Selenium | AIエージェント、文章生成、参照検索、ブラウザ自動化、再試行・品質改善 |
| **Solana / Web3** | Solana Web3.js, SPL Token, Wallet Adapter, Jupiter, Anchor Client, Rust / Pinocchio / LiteSVM | Wallet・Transaction連携、DeFi UX、Program R&D・テストの設計・連携 |
| **Cloud / Delivery** | Cloudflare, AWS, Git, GitHub, CI, Figma | Serverless運用、ログ・障害対応、PRレビュー、リリース、仕様調整 |

## 開発の進め方

1. **目的と制約を揃える** — 誰のどの課題を解くか、期限・リスク・成功条件を整理します。
2. **最小の縦切りで検証する** — UI、API、DB、外部連携をつなぎ、早い段階で動く経路を作ります。
3. **実行結果で品質を担保する** — 型、テスト、ログ、on-chain state、balance deltaを確認し、外部サービスや生成結果をそのまま信頼しません。
4. **判断を共有してShipする** — 選択肢とtrade-offを言語化し、レビュー、CI、リリース後の改善まで進めます。

## Writing & Recognition

- Zenn: [React / ViteとHonoで作るブロックチェーンアプリケーション](https://zenn.dev/yusukekikuta/articles/04904b02dcadfb)
- Colosseum Frontier Hackathon — Superteam Japan Track Winner ($4,000)
- Sol Hack3rs Global Hackathon — Slash Vision Labs Award / Audience Award ($1,000)
- Breakout Hackathon — Zee Prime Capital Sidetrack 1st Place ($25,000, 158チームから選出)

## Contact

業務委託、PoC、Technical Lead、Web / AI / Solana開発のご相談を歓迎しています。

- **Email:** [yusukekikuta.05@gmail.com](mailto:yusukekikuta.05@gmail.com)
- **LinkedIn:** [yusukekikuta](https://www.linkedin.com/in/yusukekikuta)
- **X:** [@muse_jp_sol](https://x.com/muse_jp_sol)
- **Portfolio:** [yusuke-portfolio.yusukekikuta-05.workers.dev](https://yusuke-portfolio.yusukekikuta-05.workers.dev)
