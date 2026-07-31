# Earned AI Model Optionality

**AIモデルは選べる。選べるのは、選べるようにした企業だけだ / AI Models Are Switchable. But Only for Companies That Made Them So.**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Language](https://img.shields.io/badge/Language-Japanese%20%7C%20English-blue)](docs/)

<p align="left">
  <img src="./assets/ogp_design.png" width="80%">
</p>

*Read this in other languages: [English](README_en.md)*

---

> **定義｜What is Earned AI Model Optionality**
>
> **本書とは**、山内怜史（Satoshi Yamauchi）による、AIモデルの切り替えを
> めぐる構造分析である。性能は収斂し、価格は下がり、API互換フォーマットは
> 普及した——それでもエンタープライズの年間切り替え率は11%、上位3社の
> 占有は88%にとどまる。本書はこの状態を「**獲得された選択肢（Earned
> Optionality）**」と定義する。選択肢が市場に存在していても、それを行使
> できるのは交換可能な構造を自ら構築した企業に限られる、という状態を指す。
> 接続変更・品質再評価・キャッシュ喪失・信頼回復という4つの実測コストと、
> 誰も測っていない3つの残余コストを分解し、動けている企業が平時に何を
> 作っていたのかを示す。
> 終章の言葉：「選択肢は、市場が与えるものではない。買い手が自分で獲得する
> ものである。」
>
> **This book** is a structural analysis by Satoshi Yamauchi of what it
> actually costs to switch AI models. Performance has converged, prices
> keep falling, and OpenAI-compatible formats are widespread — yet the
> enterprise switching rate is 11% per year and 88% of usage remains with
> three vendors. The book coins the term "**Earned Optionality**" for a
> state where switchability exists in the market but can only be exercised
> by buyers who built the structure themselves.
>
> **利害関係の開示 / Disclosure**：著者は特定のモデル提供者およびゲート
> ウェイ製品の販売者ではない。本書は独立分析であり、いずれのベンダーからも
> 資金提供を受けていない。The author sells neither a model provider nor a
> gateway product. This is an independent analysis with no vendor funding.
>
> *著者・全書籍一覧 / Author & full catalog: [github.com/Leading-AI-IO](https://github.com/Leading-AI-IO)*

---

## 📖 概要

Airbnbはカスタマーサービスに Alibaba の Qwen を使っている。CEO の Brian Chesky はその理由を「fast and cheap」と説明した。Cursor を開発する Anysphere は Moonshot AI の Kimi 系を採用したと報じられ、米下院委員会は両社に対する調査を開始した。**モデルは、交換された。** ここまでは、よく知られた話である。

だが同じ2026年、Menlo Ventures はまったく別のことを報告している。**ベンダー間の切り替えは比較的容易だが、ますます稀になっている。** 年間の切り替え率は11%。エンタープライズの LLM API 利用の88%は、OpenAI・Anthropic・Google の3社に集中している。
> **交換できるはずのものが、交換されていない。本書は、この矛盾から始まる。**

一見すると矛盾に見えるが、そうではない。「容易」が指しているのは接続だけだからだ。AIエージェント基盤を開発する Lindy の実測は、モデル移行の評価だけで**6〜9か月**、実際に要した労力は**当初の想定の100倍**だったと報告している。同社のエンジニアの言葉が、本書の全体を要約している——**「モデル名を変えるのは簡単だった。ユーザーが引き続き信頼するかを証明する部分が仕事だった。」**

本書は、切り替えの総コストを8項目に分解する。接続変更（LiteLLM の公開issueに記録された互換性の破れ）、品質再評価（自社の基準がなければ比較が成立しない）、キャッシュ喪失（DeepSeek 98%・Claude Sonnet 4.6 90%の割引は持ち出せない）、信頼回復（社内承認の取り直しと動機の非対称性）。そして残る3項目——安全性・法務承認、ファインチューニング資産の喪失、二重運用——について、**定量化した資料は発見できなかった。** Claude・ChatGPT・Gemini の3エンジンが独立に、同じ空白を報告している。

中心命題は一つである。**選択肢は、市場が与えるものではない。買い手が自分で獲得するものである。** 抽象化レイヤー、常設された評価、維持されたフォールバック——動けている企業が持っていた3つは、いずれも平時に払うコストだった。切り替えが必要になった時点では、もう間に合わない。本書は、価格が下がっているのに買い手が動かない市場で、何が交渉力の正体なのかを問うOSS書籍である。

---

## 📄 ドキュメント

| ファイル | 言語 | 内容 |
| --- | --- | --- |
| [earned-ai-model-optionality_JP.md](./docs/jp/earned-ai-model-optionality_JP.md) | 🇯🇵 日本語 | 本文（日本語版） |
| [earned-ai-model-optionality_EN.md](./docs/en/earned-ai-model-optionality_EN.md) | 🇺🇸 English | 本文（英語版） |

---

## 📑 目次

- **序章:** 交換できるはずだった
- **第1章:** 88%は、動いていない
- **第2章:** 互換と書いてある。互換ではない
- **第3章:** 6ヶ月と、100倍の労力
- **第4章:** 安くなるほど、動けなくなる
- **第5章:** ユーザーが信頼するかを、証明する仕事
- **第6章:** 残りのコストは、誰も測っていない
- **第7章:** 選べる企業は、何を作ったのか
- **第8章:** 日本企業は、選べる側にいるか
- **終章:** 選択肢は、獲得するものである

---

## 🔗 Related Projects

本書は、以下のOSSプロジェクトと相互に接続されている。

| プロジェクト | 概要 | リンク |
| --- | --- | --- |
| **The AI Strategist**               | AIストラテジストという職業を定義し、BTC交差点で戦うための実践的フレームワーク    | [GitHub](https://github.com/Leading-AI-IO/the-ai-strategist)              |
| **Depth & Velocity**                | 生成AI時代の新規事業開発方法論                             | [GitHub](https://github.com/Leading-AI-IO/depth-and-velocity)             |
| **The Silence of Intelligence**     | Anthropic CEO ダリオ・アモディの思想を体系化。産業構造の解剖シリーズ第2弾 | [GitHub](https://github.com/Leading-AI-IO/the-silence-of-intelligence)    |
| **The Anatomy of Anthropic**        | Anthropicの戦略・製品・研究・安全性を包括的に解剖                | [GitHub](https://github.com/Leading-AI-IO/the-anatomy-of-anthropic)       |
| **The Palantir Impact**             | Palantir Foundryのオントロジー戦略を解剖。産業構造の解剖シリーズ第1弾  | [GitHub](https://github.com/Leading-AI-IO/palantir-ontology-strategy)     |
| **What They Won't Teach You**       | AIに有利な世代が教えない、AIの使い方と"思考のOS"                 | [GitHub](https://github.com/Leading-AI-IO/what-they-wont-teach-you)       |
| **The Edge of Intelligence**        | AIがあなたのデバイスで動く時代：クラウドの終わりと、エッジの始まり           | [GitHub](https://github.com/Leading-AI-IO/edge-ai-intelligence)           |
| **The Redesign of Design Strategy** | デザイン戦略の再定義。IDEO崩壊の構造分析を含む                    | [GitHub](https://github.com/Leading-AI-IO/design-strategy-in-the-ai-era)  |
| **The Orchestrator**                | AI時代に最も希少な人材像「オーケストレーター」を世界で初めて定義            | [GitHub](https://github.com/Leading-AI-IO/the-orchestrator-in-the-ai-era) |
| **Advertising, Redesigned**         | AI時代の広告の未来を、7社の戦略と構造分析から描くOSS書籍              | [GitHub](https://github.com/Leading-AI-IO/advertising-redesigned)         |
| **The AI Organization**             | AI導入が失敗する本質は技術ではなく組織にある。AI時代の組織論      | [GitHub](https://github.com/Leading-AI-IO/the-ai-organization)  |
| **The Structural Shift from SaaS**  | SaaSからService-as-a-Softwareへの構造的転換。Next SaaS ビジネスモデル。      | [GitHub](https://github.com/Leading-AI-IO/saas-is-dead-the-next-ai-business-model)  |
| **The 10:80:10 Principle**          | 人とAIの共創黄金比「10:80:10」の法則——AI時代の思考のOS。      | [GitHub](https://github.com/Leading-AI-IO/the-10-80-10-principle)  |
| **A Trillion Dollars and a Firebomb** | 1兆ドルと火炎瓶。AI時代の同時加速する現実。 | [GitHub](https://github.com/Leading-AI-IO/a-trillion-and-a-firebomb)  |
| **The End of the Attention Economy** | アテンション・エコノミーの終わり。次世代SNSの在り方とは？ | [GitHub](https://github.com/Leading-AI-IO/the-attention-economy-is-over)  |
| **The Growth Engine of Anthropic** | Anthropicの1兆ドル到達の構造解剖。 | [GitHub](https://github.com/Leading-AI-IO/the-growth-engine-of-anthropic)  |
| **The Agentic Commerce Economy** | AIエージェントが購買を代行する時代、広告モデルの構造的変化。 | [GitHub](https://github.com/Leading-AI-IO/agentic-commerce-economy)  |
| **Will ai break the planet** | 数十兆円のインフラ投資と、地球温暖化の「不可逆ライン」。 | [GitHub](https://github.com/Leading-AI-IO/will-ai-break-the-planet)  |
| **The-forward-deployed-shift** | 成果実装 ── FDEが示す、AIで「作る」が終わった世界の価値のありか。 | [GitHub](https://github.com/Leading-AI-IO/the-forward-deployed-shift)  |
| **Frontier-Grade Open Weights** | 特権的なオープン。移動したのは所有権ではなく希少性の在処である。 | [GitHub](https://github.com/Leading-AI-IO/frontier-grade-open-weights)  |

---

## 👤 著者

**Satoshi Yamauchi** (山内 怜史)

* **AI Strategist & Business Designer at Sun Asterisk Inc.**

* **Founder / AI Strategist at [Leading.AI](https://www.leading-ai.io/)**

* 15年以上にわたりBusiness・Technology・Creativeの3領域を越境。フューチャーアーキテクトでITコンサルタントとして40案件のPL/PMを推進後、リクルートで事業戦略・新規事業開発に従事。Sun Asteriskでビジネスデザイナー兼AIストラテジストとして、新規事業×生成AIの方法論「Depth & Velocity」を体系化。

* This project is part of the research by Leading.AI.

* [📒 Read my insights on Note](https://note.com/satoshi_yamauchi)

* [🌐 Visit Leading.AI Official Website](https://www.leading-ai.io/)

---

## 🤝 Contributing

Issues and Pull Requests are welcome. 本書の構造分析に対するフィードバック、モデル切り替えの実測データ（期間・工数・失敗事例）、抽象化レイヤー／評価基盤／フォールバック運用の実装知見、AIモデル調達の標準手順に関する一次資料、誤字脱字の修正、翻訳へのContributeを歓迎します。特に、本書が「測られていない」と記した3項目——安全性・法務承認、ファインチューニング資産の喪失、移行期間中の二重運用——の定量データをお持ちの方からの情報提供を求めています。

---

## 📝 License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).<br>
© 2026 Satoshi Yamauchi / [Leading AI](https://www.leading-ai.io/) — Licensed under CC BY 4.0
