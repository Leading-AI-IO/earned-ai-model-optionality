# Earned AI Model Optionality

**AI Models Are Switchable. But Only for Companies That Made Them So.**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Language](https://img.shields.io/badge/Language-Japanese%20%7C%20English-blue)](docs/)

<p align="left">
  <img src="./assets/ogp_design.png" width="80%">
</p>

*Read this in other languages: [日本語](README.md)*

---

> **Definition**
>
> **This book** is a structural analysis by Satoshi Yamauchi (山内怜史), AI
> Strategist, of what it actually costs to switch AI models. Performance
> has converged, prices keep falling, and OpenAI-compatible formats are
> widespread — yet the enterprise switching rate is 11% per year and 88%
> of enterprise LLM API usage remains with three vendors. The book coins
> the term "**Earned Optionality**" for a state in which the possibility
> of switching exists in the market, but the ability to exercise it is
> limited to buyers who built a switchable structure themselves. It
> decomposes four measured costs — connection changes, quality
> re-evaluation, loss of caching, and restoring trust — alongside three
> costs no one has measured, and shows what the companies that can still
> move had already built in peacetime. As stated in the closing chapter:
> "Optionality is not something the market gives. It is something the
> buyer earns."
>
> **Disclosure**: The author sells neither a model provider nor a gateway
> product. This is an independent analysis with no vendor funding.
>
> *Author & full catalog: [github.com/Leading-AI-IO](https://github.com/Leading-AI-IO)*

---

## 📖 Overview

Airbnb uses Alibaba's Qwen for customer service; CEO Brian Chesky explained the reason as "fast and cheap." Anysphere, the company behind Cursor, was reported to have adopted Moonshot AI's Kimi family, and House committees opened an investigation into both companies. **The models were switched.** Up to this point, the story is well known.

Yet in that same year, 2026, Menlo Ventures reported something entirely different. **Switching between vendors is relatively easy, but it is becoming increasingly rare.** The annual switching rate is 11%. And 88% of enterprise LLM API usage is concentrated in three companies: OpenAI, Anthropic, and Google.

**What is supposed to be switchable is not being switched. This book begins from that contradiction.**

The contradiction is only apparent. What "easy" refers to is the connection alone. Lindy, which builds an AI agent platform, measured **six to nine months for evaluation alone**, with the actual migration requiring **100 times the initial estimate** in effort. An engineer's words summarize the entire book: **"Changing the model name was easy. The work was proving that users would still trust it."**

This book decomposes the total cost of switching into eight items: connection changes (compatibility breaks documented in LiteLLM's public issues), quality re-evaluation (no comparison is possible without a standard of your own), loss of caching (the 98% discount on DeepSeek and 90% on Claude Sonnet 4.6 cannot be carried out), and restoring trust (re-obtaining internal approvals, and the asymmetry of incentives). About the remaining three — safety and legal approval, loss of fine-tuning assets, and dual running during migration — **no material quantifying them could be found.** Three research engines, Claude, ChatGPT, and Gemini, independently reported the same blank.

Its central thesis is simple: **optionality is not something the market gives; it is something the buyer earns.** An abstraction layer, standing evaluation, and a maintained fallback — the three things the movers held were all costs paid in peacetime. By the time switching becomes necessary, it is already too late. This open-source book asks what leverage actually consists of, in a market where prices are falling and buyers still do not move.

---

## 📄 Document

| File | Language | Content |
| --- | --- | --- |
| [earned-ai-model-optionality_JP.md](./docs/jp/earned-ai-model-optionality_JP.md) | 🇯🇵 Japanese | Full text (Japanese edition) |
| [earned-ai-model-optionality_EN.md](./docs/en/earned-ai-model-optionality_EN.md) | 🇺🇸 English | Full text (English edition) |

---

## 📑 Table of Contents

- **Prologue:** They Were Supposed to Be Switchable
- **Chapter 1:** 88% Are Not Moving
- **Chapter 2:** It Says Compatible. It Is Not Compatible.
- **Chapter 3:** Six Months, and 100× the Effort
- **Chapter 4:** The Cheaper It Gets, the Less You Can Move
- **Chapter 5:** The Work of Proving That Users Still Trust It
- **Chapter 6:** Nobody Has Measured the Remaining Costs
- **Chapter 7:** What Did the Companies That Can Choose Actually Build?
- **Chapter 8:** Are Japanese Companies on the Side That Can Choose?
- **Final Chapter:** Optionality Is Something You Earn

---

## 🔗 Related Projects

This book is part of an interconnected ecosystem of open-source projects.

| Project | Description | Link |
| --- | --- | --- |
| **The AI Strategist**               | Defining the AI Strategist role with practical frameworks for the BTC intersection                              | [GitHub](https://github.com/Leading-AI-IO/the-ai-strategist)              |
| **Depth & Velocity**                | A methodology for new business development in the generative AI era                                             | [GitHub](https://github.com/Leading-AI-IO/depth-and-velocity)             |
| **The Silence of Intelligence**     | Systematizing Anthropic CEO Dario Amodei's philosophy — Industry Anatomy Series #2                              | [GitHub](https://github.com/Leading-AI-IO/the-silence-of-intelligence)    |
| **The Anatomy of Anthropic**        | A comprehensive dissection of Anthropic's strategy, products, research, and safety                              | [GitHub](https://github.com/Leading-AI-IO/the-anatomy-of-anthropic)       |
| **The Palantir Impact**             | Dissecting Palantir Foundry's ontology strategy — Industry Anatomy Series #1                                    | [GitHub](https://github.com/Leading-AI-IO/palantir-ontology-strategy)     |
| **What They Won't Teach You**       | What the AI-advantaged generation won't teach you about AI and the "Thinking OS"                                | [GitHub](https://github.com/Leading-AI-IO/what-they-wont-teach-you)       |
| **The Edge of Intelligence**        | When AI runs on your device: the end of cloud, the beginning of edge                                            | [GitHub](https://github.com/Leading-AI-IO/edge-ai-intelligence)           |
| **The Redesign of Design Strategy** | Redefining design strategy, including a structural analysis of IDEO's decline                                   | [GitHub](https://github.com/Leading-AI-IO/design-strategy-in-the-ai-era)  |
| **The Orchestrator**                | The first-ever definition of the rarest role in the AI era                                                      | [GitHub](https://github.com/Leading-AI-IO/the-orchestrator-in-the-ai-era) |
| **Advertising, Redesigned**         | An open-source book exploring the future of advertising in the AI era through strategic analysis of 7 companies | [GitHub](https://github.com/Leading-AI-IO/advertising-redesigned)         |
| **The AI Organization**             | The root cause of AI failure is not technology. Organizational theory for the AI era                            | [GitHub](https://github.com/Leading-AI-IO/the-ai-organization)  |
| **The Structural Shift from SaaS**  | SaaS Is Dead: The Structural Shift from SaaS to Service-as-a-Software                                           | [GitHub](https://github.com/Leading-AI-IO/saas-is-dead-the-next-ai-business-model)  |
| **The 10:80:10 Principle**          | The optimal balance for human-AI synergy:「10:80:10」in the AI era.                                             | [GitHub](https://github.com/Leading-AI-IO/the-10-80-10-principle)  |
| **A Trillion Dollars and a Firebomb** | The Parallel Realities of the AI Era | [GitHub](https://github.com/Leading-AI-IO/a-trillion-and-a-firebomb) |
| **The End of the Attention Economy** | The End of the Attention Economy. What Should the Next SNS Look Like? | [GitHub](https://github.com/Leading-AI-IO/the-attention-economy-is-over)  |
| **The Growth Engine of Anthropic** | Decoding the $1T Trajectory | [GitHub](https://github.com/Leading-AI-IO/the-growth-engine-of-anthropic)  |
| **The Agentic Commerce Economy** | When AI Agents Buy, the Advertising Model Paradigm Shift | [GitHub](https://github.com/Leading-AI-IO/agentic-commerce-economy)  |
| **Will ai break the planet** | The AI Infrastructure Boom and the Race Against the Climate's Point of No Return | [GitHub](https://github.com/Leading-AI-IO/will-ai-break-the-planet)  |
| **The-forward-deployed-shift** | The Forward Deployed Shift — Where Value Survives When "Building" Is Over | [GitHub](https://github.com/Leading-AI-IO/the-forward-deployed-shift)  |
| **Frontier-Grade Open Weights** | Privileged Open — what moved was not ownership but the location of scarcity | [GitHub](https://github.com/Leading-AI-IO/frontier-grade-open-weights)  |

---

## 👤 Author

**Satoshi Yamauchi** (山内 怜史)<br>

* **AI Strategist & Business Designer at Sun Asterisk Inc.**

* **Founder / AI Strategist at [Leading.AI](https://www.leading-ai.io/)**

* Over 15 years of experience spanning Business, Technology, and Creative domains. Led 40+ projects as PL/PM at Future Architect (IT consulting), then drove business strategy and new business development at Recruit. Currently at Sun Asterisk as a Business Designer and AI Strategist, where he developed “Depth & Velocity”—a methodology for new business development powered by generative AI.

* This project is part of the research by Leading.AI.

* [📒 Read my insights on Note](https://note.com/satoshi_yamauchi)

* [🌐 Visit Leading.AI Official Website](https://www.leading-ai.io/)

---

## 🤝 Contributing

Issues and Pull Requests are welcome. Contributions are appreciated, including feedback on the book's structural analysis; measured data on model migrations (duration, effort, failure cases); implementation knowledge on abstraction layers, evaluation platforms, and fallback operations; primary sources on standard procedures for AI model procurement; corrections; and translations. In particular, we are seeking quantitative data on the three items this book describes as unmeasured — safety and legal approval, loss of fine-tuning assets, and dual running during migration.

---

## 📝 License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).<br>
© 2026 Satoshi Yamauchi / [Leading AI](https://www.leading-ai.io/) — Licensed under CC BY 4.0
