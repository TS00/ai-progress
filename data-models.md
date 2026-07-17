# Frontier AI/LLM Model Releases — June 2020 to July 2026

A structured, sourced compilation of significant frontier model releases from GPT‑3 through July 9, 2026.

## Methodology and caveats

- **Scope**: "frontier" releases only — models that set or contested state of the art at release, plus the most influential open‑weights drops. Minor checkpoints (e.g., dated revisions, mini/nano variants) are noted in the parent row rather than given their own entry, except where they had distinct strategic importance.
- **Compute (FLOP)** and **training cost (USD)** for closed models are almost never officially disclosed. Numbers come primarily from the [Epoch AI Notable AI Models database](https://epoch.ai/data/ai-models) and their [>1e25 FLOP tracker](https://epoch.ai/data-insights/models-over-1e25-flop). Most are imputed from benchmarks or estimated from hardware × duration; treat them as **order‑of‑magnitude estimates**.
- **Parameter counts** for closed models are unconfirmed unless sourced from the developer. Where third‑party leaks are the only source, they are flagged as such.
- **Benchmarks** are reported as the developer or independent evaluator stated them at release. Different harnesses, prompt scaffolds, tool budgets, and "thinking" modes are not directly comparable across rows; numbers are indicative, not definitive. Where multiple modes exist (e.g. "high"/"thinking"/"pro"), the strongest publicly reported number is shown.
- "OW" = open‑weights, "C" = closed.
- "≈" = approximate, "—" = not disclosed / not applicable / no comparable benchmark at the time.
- Today's date: **July 9, 2026**.

---

## Master timeline (chronological summary)

| Date | Model | Developer | Why it mattered |
|---|---|---|---|
| 2020‑06 | GPT‑3 | OpenAI | First 175B dense LM; defined the modern LLM era |
| 2022‑04 | PaLM 540B | Google | Largest dense LM at the time; chain‑of‑thought emergence |
| 2022‑11 | ChatGPT (GPT‑3.5) | OpenAI | RLHF + product moment; AI consumer wave |
| 2023‑03 | GPT‑4 | OpenAI | First clearly post‑GPT‑3.5 frontier; >1e25 FLOP era |
| 2023‑03 | Claude 1 | Anthropic | First Claude; Constitutional AI |
| 2023‑02 | LLaMA 1 | Meta | Sparked the open‑weights ecosystem |
| 2023‑05 | PaLM 2 | Google | Multilingual + code‑heavy successor |
| 2023‑07 | Llama 2 | Meta | First commercially licensable open‑weights frontier |
| 2023‑11 | GPT‑4 Turbo | OpenAI | 128K context, cheaper, JSON mode |
| 2023‑12 | Gemini 1.0 (Ultra/Pro) | Google DeepMind | First Gemini; natively multimodal |
| 2023‑12 | Mixtral 8x7B | Mistral | Popularized open MoE |
| 2024‑02 | Gemini 1.5 Pro | Google DeepMind | 1M‑token context (later 2M) |
| 2024‑03 | Claude 3 (Haiku/Sonnet/Opus) | Anthropic | Reclaimed frontier from GPT‑4 on many evals |
| 2024‑04 | Llama 3 (8B/70B) | Meta | Best open‑weights at release |
| 2024‑05 | GPT‑4o | OpenAI | Native multimodal (text/vision/audio) |
| 2024‑06 | Claude 3.5 Sonnet | Anthropic | Cheap+strong; reset the curve |
| 2024‑07 | Llama 3.1 405B | Meta | First open‑weights model at GPT‑4‑class scale |
| 2024‑07 | Mistral Large 2 (123B) | Mistral | Strongest mid‑size open‑weights of 2024 |
| 2024‑09 | o1‑preview / o1 | OpenAI | First production reasoning model |
| 2024‑12 | Gemini 2.0 Flash | Google DeepMind | Cheap multimodal; thinking mode preview |
| 2024‑12 | DeepSeek V3 (671B MoE) | DeepSeek | Frontier open‑weights at ~$5.6M training cost |
| 2024‑12 | o3 announcement | OpenAI | 87.5% ARC‑AGI‑1; 25.2% FrontierMath |
| 2025‑01 | DeepSeek R1 | DeepSeek | First open‑weights reasoning model at o1 level |
| 2025‑02 | Claude 3.7 Sonnet | Anthropic | First Anthropic hybrid reasoning model |
| 2025‑02 | GPT‑4.5 ("Orion") | OpenAI | Largest pre‑trained OpenAI model |
| 2025‑03 | Gemini 2.5 Pro | Google DeepMind | Native thinking; #1 LMArena |
| 2025‑04 | Llama 4 (Scout/Maverick) | Meta | First open‑weights MoE; 10M context (Scout) |
| 2025‑04 | o3 (full) / o4‑mini | OpenAI | Reasoning + tool use as default |
| 2025‑05 | Claude 4 (Opus/Sonnet) | Anthropic | Long agentic horizons (>30h coding) |
| 2025‑07 | Grok 4 | xAI | First model >50% on Humanity's Last Exam (Heavy) |
| 2025‑07 | Kimi K2 (1T MoE) | Moonshot AI | First open‑weights 1T MoE; agentic SOTA at OSS |
| 2025‑08 | GPT‑5 | OpenAI | Unified router + reasoning; new SOTA at release |
| 2025‑08 | Claude Opus 4.1 | Anthropic | 74.5% SWE‑bench Verified |
| 2025‑08 | DeepSeek V3.1 | DeepSeek | Hybrid reason/non‑reason in one model |
| 2025‑09 | Claude Sonnet 4.5 | Anthropic | Best agentic + computer‑use model at release |
| 2025‑09 | Qwen3‑Max (1T+ MoE) | Alibaba | Alibaba's first trillion‑parameter flagship |
| 2025‑11 | Gemini 3 Pro | Google DeepMind | New SOTA across reasoning, coding, multimodal |
| 2025‑11 | Kimi K2 Thinking | Moonshot AI | First OSS to exceed GPT‑5 on multiple agentic evals |
| 2025‑11 | GPT‑5.1 / 5.1 Pro / Codex‑Max | OpenAI | Personality + agentic coding |
| 2025‑11 | Claude Opus 4.5 | Anthropic | Lower price tier; near‑#1 Intelligence Index |
| 2025‑12 | GPT‑5.2 | OpenAI | Rapid follow‑up to Gemini 3; xhigh reasoning effort |
| 2025‑12 | DeepSeek V3.2 / V3.2‑Speciale | DeepSeek | Sparse Attention; gold‑medal IMO/IOI |
| 2025‑12 | Mistral Large 3 | Mistral | Open Apache‑2.0 675B MoE |
| 2026‑01 | Qwen3‑Max‑Thinking | Alibaba | Test‑time scaling, ties frontier on HLE |
| 2026‑02 | Gemini 3.1 Pro / Deep Think | Google DeepMind | 77% ARC‑AGI‑2; 65K output tokens |
| 2026‑02 | GPT‑5.3 / 5.3‑Codex | OpenAI | Codex specialization |
| 2026‑03 | GPT‑5.4 (Thinking/Pro) | OpenAI | Unified Codex + agentic |
| 2026‑04 | Claude Mythos Preview | Anthropic | First "Mythos‑class" model; restricted to Project Glasswing cyberdefenders |
| 2026‑04 | Muse Spark | Meta (MSL) | First Meta Superintelligence Labs model; Meta's first closed frontier release |
| 2026‑04 | DeepSeek V4 (Pro/Flash) | DeepSeek | 1.6T MoE; native 1M context, MIT |
| 2026‑04 | Kimi K2.6 GA | Moonshot AI | 12‑hour coding runs, 300‑agent swarms |
| 2026‑04 | GPT‑5.5 | OpenAI | Fully retrained agentic model |
| 2026‑05 | Llama 5 (8B / Scout 109B) | Meta | Meta's open comeback; native vision+audio |
| 2026‑05 | Gemini 3.5 Flash + Gemini Omni | Google DeepMind | Flash tier beats 3.1 Pro on agentic/coding; first unified any‑to‑any multimodal |
| 2026‑05 | Qwen 3.7 Max | Alibaba | Alibaba's agentic API flagship |
| 2026‑05 | Claude Opus 4.8 | Anthropic | SWE‑bench Pro 69.2%; Dynamic Workflows (100s of parallel subagents) |
| 2026‑06 | Qwen 4 (open, 32B‑A3B + Coder) | Alibaba | Apache‑2.0; frontier‑adjacent coding on consumer hardware |
| 2026‑06 | Llama 5 70B / Mistral Voyage Pro 70B | Meta / Mistral | 70B‑dense tier competitive again; same‑day release |
| 2026‑06 | Grok 4 Open | xAI/SpaceXAI | xAI's first‑ever open‑weights release (100B‑A20B) |
| 2026‑06 | Claude Fable 5 / Mythos 5 | Anthropic | First GA Mythos‑class model; suspended Jun 12 by US export controls, restored Jul 1 |
| 2026‑06 | Kimi K2.7‑Code | Moonshot AI | Coding‑specialist open 1T MoE |
| 2026‑06 | Claude Sonnet 5 | Anthropic | Near‑Opus‑4.8 agentic performance at $2/$10 |
| 2026‑07 | Grok 4.5 | xAI/SpaceXAI | "Opus‑class" at $2/$6; 2× token efficiency; trained alongside Cursor |
| 2026‑07 | GPT‑5.6 (Sol/Terra/Luna) | OpenAI | New SOTA family; first gov‑gated preview before GA; `ultra` multi‑agent mode |
| 2026‑07 | Muse Spark 1.1 | Meta (MSL) | Meta's return to the frontier pack; multimodal agentic model + first paid Meta Model API |

---

## OpenAI

| Model | Release | Params | Compute (FLOP) | Training cost | Context | OW/C | Key benchmarks | Significance |
|---|---|---|---|---|---|---|---|---|
| **GPT‑3** (`davinci`) | 2020‑06‑11 | 175B dense | ≈3.1e23 (Epoch AI) | ≈$4.6M (early estimates) | 2K | C | MMLU 43.9% (5‑shot, paper) | First web‑scale LLM that worked; few‑shot prompting paradigm |
| **GPT‑3.5 / ChatGPT** | 2022‑11‑30 | ≈175B (`text‑davinci‑003` lineage) | — | — | 4K → 16K | C | MMLU ≈70%, HumanEval 48% | RLHF + product launch; ignited the LLM consumer wave |
| **GPT‑4** | 2023‑03‑14 | Undisclosed (≈1.8T MoE per leaks; unconfirmed) | **2.1e25** (Epoch AI low‑precision) | $40–100M (commonly cited; Epoch range) | 8K → 32K | C | MMLU 86.4%, HumanEval 67%, GPQA 35.7% | First clearly post‑3.5 frontier; multimodal vision later |
| **GPT‑4 Turbo** (`gpt‑4‑1106`) | 2023‑11‑06 | — | **2.2e25** | — | 128K | C | MMLU ≈86%, HumanEval ≈85% | 128K context, JSON mode, cheaper |
| **GPT‑4o** ("omni") | 2024‑05‑13 | — | **3.8e25** | — | 128K | C | MMLU 88.7%, HumanEval 90.2%, GPQA 53.6%, MMMU 69.1% | Native text+vision+audio; voice mode |
| **o1‑preview** | 2024‑09‑12 | — | — | — | 128K | C | AIME 2024 56.7%, GPQA 78%, MATH 85% | First production reasoning model (RL on chain‑of‑thought) |
| **o1** | 2024‑12‑05 | — | — | — | 200K | C | AIME 2024 83.3%, GPQA 75.7%, MATH ≈94% | Replaced o1‑preview; ChatGPT Pro tier ($200/mo) |
| **o3** (preview) | 2024‑12‑20 → GA 2025‑04‑16 | — | — | — | 200K | C | ARC‑AGI‑1 87.5% (high‑compute), 75.7% (low); FrontierMath 25.2%; SWE‑bench 71.7%; AIME 96.7% | Step‑change in agentic + math reasoning; ARC breakthrough |
| **o3‑mini** | 2025‑01‑31 | — | — | — | 200K | C | AIME 87.3%, Codeforces 2073 Elo | Cheap reasoning for masses |
| **o4‑mini** | 2025‑04‑16 | — | — | — | 200K | C | AIME 2025 ≈93%, GPQA ≈81% | Efficient reasoner; multimodal |
| **GPT‑4.1** | 2025‑04‑14 | — | "Speculative" >1e25 (Epoch) | — | 1M | C | SWE‑bench 54.6%, MMMU 75.6% | Long‑context, cheaper, dev‑first |
| **GPT‑4.5** ("Orion") | 2025‑02‑27 | — | **6.4e25** (Epoch) | "Several hundred million" (rumored) | 128K | C | MMLU‑Pro 84%, GPQA ≈71% | Largest pre‑trained OpenAI model; effectively retired by GPT‑5 |
| **GPT‑5** | 2025‑08‑07 | — | — (likely >1e26) | — | **400K** (272K in / 128K out) | C | AIME 2025 94.6% (no tools), SWE‑bench Verified 74.9%, MMMU 84.2%, GPQA 88.4% (Pro), Aider Polyglot 88% | Unified router + reasoning model; Pro tier with parallel test‑time compute |
| **GPT‑5.1** (Instant/Thinking/Pro/Codex‑Max) | 2025‑11‑12 (5.1 Pro & Codex‑Max 11‑19) | — | — | — | 400K | C | SWE‑bench Verified 76.3%, GPQA ≈90%, ARC‑AGI‑2 17.6% | Personality customization, longer agentic coding (24h Codex‑Max task internally) |
| **GPT‑5.2** (Instant/Thinking/Pro, Codex) | 2025‑12‑11 | — | — | — | 400K | C | SWE‑bench Verified ≈80%, GPQA 92.4%, HLE 34.5%, ARC‑AGI‑2 52.9%, LiveCodeBench Pro 2393 Elo | Released 3 weeks after Gemini 3 ("Code Red"); xhigh reasoning effort |
| **GPT‑5.3‑Codex** | 2026‑02‑05 | — | — | — | 400K | C | SWE‑bench Pro 56.8%, Terminal‑Bench 2.0 64.7–77.3% (Codex harness) | Coding specialization |
| **GPT‑5.4** (Thinking / Pro / mini) | 2026‑03‑05 | — | — | — | 400K | C | Codex‑class agentic + spreadsheet/slide work | Unified Codex strengths back into mainline |
| **GPT‑5.5** | 2026‑04‑23 | — | — | — | 400K | C | Terminal‑Bench 2.0 82.7%, GDPval 84.9%, SWE‑bench Pro ≈58.6% (single‑pass) | Fully retrained agentic model; #1 Artificial Analysis Index at release |
| **GPT‑5.6 (Sol / Terra / Luna)** | Preview 2026‑06‑26 → GA **2026‑07‑09** | — | — | — | 400K | C | Sol: Terminal‑Bench 2.1 88.8% (91.9% ultra), SWE‑bench Pro 64.6%, BrowseComp 90.4% (92.2% ultra), OSWorld 2.0 62.6%, GPQA Diamond 94.6%, FrontierMath T1‑3 89% / T4 83%, AA Coding Agent Index 80 (new SOTA), Agents' Last Exam 52.7 | New naming scheme (Sol=flagship, Terra=balanced, Luna=cheap); new `max` and `ultra` (4 parallel agents) settings; preview was limited to government‑vetted partners at US government request — first "government‑gated" frontier release. $5/$30, $2.50/$15, $1/$6 per Mtok |

Note: OpenAI's June 26 preview marked a new deployment pattern — at the US government's request GPT‑5.6 launched first to a small set of vetted partners (citing frontier cyber capability: ExploitBench 73.5% vs GPT‑5.5's 47.9%), with GA following two weeks later alongside a hardware‑passkey "Trusted Access for Cyber" program.

Sources: [OpenAI release notes](https://help.openai.com/en/articles/6825453-chatgpt-release-notes), [GPT‑5 announcement](https://openai.com/index/introducing-gpt-5/), [GPT‑5 for developers](https://openai.com/index/introducing-gpt-5-for-developers/), [GPT‑5.2 announcement](https://openai.com/index/introducing-gpt-5-2/), [GPT‑5.6 announcement](https://openai.com/index/gpt-5-6), [GPT‑5.6 Sol preview](https://openai.com/index/previewing-gpt-5-6-sol/), [Wikipedia: GPT‑5](https://en.wikipedia.org/wiki/GPT-5), [Wikipedia: o3](https://en.wikipedia.org/wiki/OpenAI_o3), [ARC Prize on o3](https://arcprize.org/blog/oai-o3-pub-breakthrough), [Epoch AI tracker](https://epoch.ai/data-insights/models-over-1e25-flop), [MarkTechPost: GPT‑5.5](https://www.marktechpost.com/2026/04/23/openai-releases-gpt-5-5-a-fully-retrained-agentic-model-that-scores-82-7-on-terminal-bench-2-0-and-84-9-on-gdpval/).

---

## Anthropic

| Model | Release | Params | Compute (FLOP) | Training cost | Context | OW/C | Key benchmarks | Significance |
|---|---|---|---|---|---|---|---|---|
| **Claude 1** | 2023‑03‑14 | — | — | — | 9K → 100K (1.3) | C | MMLU ≈75%, HumanEval ≈55% | First Claude; Constitutional AI |
| **Claude 2** | 2023‑07‑11 | — | — | — | 100K | C | MMLU 78.5%, HumanEval 71.2%, GSM8K 88% | First widely available 100K‑token model |
| **Claude 2.1** | 2023‑11‑21 | — | — | — | 200K | C | — | 200K context, tool‑use beta |
| **Claude 3 Haiku / Sonnet / Opus** | 2024‑03‑04 | — | Opus **1.6e25** (Epoch) | "Tens of millions" | 200K | C | Opus: MMLU 86.8%, HumanEval 84.9%, GPQA 50.4%, MATH 60.1%, MMMU 59.4% | Reclaimed top spot from GPT‑4 on many evals |
| **Claude 3.5 Sonnet** | 2024‑06‑20 (`20240620`); refresh 2024‑10‑22 | — | **3.6e25** (Epoch) | "A few $10Ms" (Amodei) | 200K | C | MMLU‑Pro 78%, HumanEval 92%, GPQA 65%, SWE‑bench 49%, MATH 78.3% | Sonnet ≥ prior Opus at lower price; reset cost/quality curve |
| **Claude 3.5 Haiku** | 2024‑11‑04 | — | — | — | 200K | C | SWE‑bench 40.6% | Cheap, fast |
| **Claude 3 Opus 3.5** (cancelled) | — | — | — | — | — | — | — | Internal codename for what became Sonnet 3.5 retraining; never shipped as Opus |
| **Claude 3.7 Sonnet** | 2025‑02‑24 | — | **3.4e25** (Epoch) | "A few tens of millions" | 200K | C | SWE‑bench 70.3%, GPQA 84.8%, AIME 80% (extended thinking), MATH 96.2% | First hybrid reasoning model from Anthropic ("extended thinking") |
| **Claude Sonnet 4** | 2025‑05‑22 | — | **≈5.0e25** (Epoch est.) | — | 200K → 1M (later) | C | SWE‑bench 72.7%, GPQA 75% | Faster + smarter than 3.7 |
| **Claude Opus 4** | 2025‑05‑22 | — | — | — | 200K | C | SWE‑bench 72.5%, GPQA 79.6%, MMMU 76.5% | Anthropic's first AI Safety Level 3 (ASL‑3) deployment |
| **Claude Opus 4.1** | 2025‑08‑05 | — | — | — | 200K | C | SWE‑bench Verified 74.5%, GPQA Diamond ≈92%, AIME ≈83% (extended) | Multi‑file refactor; same price as Opus 4 |
| **Claude Sonnet 4.5** | 2025‑09‑29 | — | — | — | 200K | C | SWE‑bench Verified 77.2–82.0%, OSWorld 61.4%, Terminal‑Bench ≈50% | "Best computer‑use model"; 30+ hour autonomous coding |
| **Claude Haiku 4.5** | 2025‑10‑01 | — | — | — | 200K | C | Near‑frontier at fastest tier | Cheap reasoning |
| **Claude Opus 4.5** | 2025‑11‑24 | — | — | — | 200K | C | SWE‑bench Verified 80.9%, Terminal‑Bench 59.3%, ARC‑AGI‑2 37.6%, GPQA ≈87%, HLE w/ search ≈43%, MMLU‑Pro 90% | #2 on Artificial Analysis Intelligence Index (70); price cut to $5/$25 |
| **Claude Sonnet 4.6 / Opus 4.6** | 2025‑Q4 / 2026‑02‑05 | — | — | — | 1M | C | SWE‑bench Verified 79.6% (Sonnet 4.6) / 80.8% (Opus 4.6); ARC‑AGI‑2 58.3 / 68.8 | First Claude with 1M context; longer max output (128K Opus) |
| **Claude Mythos Preview** | 2026‑04‑07 (restricted) | — | — | — | 1M | C (Glasswing partners only) | SWE‑bench Pro 77.8% (vendor scaffold), GPQA 94.6%, BrowseComp 87.9% | First "Mythos‑class" model (tier above Opus); released only to ~40 vetted cyberdefense orgs via **Project Glasswing** in collaboration with US government |
| **Claude Opus 4.7** | 2026‑04‑16 | — | — | — | 1M | C | SWE‑bench Verified 87.6%, SWE‑bench Pro 64.3%, GPQA Diamond 94.2%, Terminal‑Bench 69.4% | "Step‑change improvement"; xhigh effort level; 3× vision resolution |
| **Claude Opus 4.8** | 2026‑05‑28 | — | — | — | 1M | C | SWE‑bench Pro 69.2%, SWE‑bench Verified 88.6%, Terminal‑Bench 2.1 74.6%, OSWorld‑Verified 83.4%, BrowseComp 84.3%, GPQA 93.6%, GDPval‑AA 1890 Elo | Dynamic Workflows (hundreds of parallel subagents), Effort Control, fast mode; same $5/$25; announced alongside Series H at $965B valuation |
| **Claude Fable 5 / Mythos 5** | 2026‑06‑09; suspended 06‑12 (US export‑control directive); restored 06‑30/07‑01 | — | — | — | 1M | C | SWE‑bench Pro 80.0/80.3% (vendor scaffold), Terminal‑Bench 2.1 83.1% (Fable) / 88% (Mythos), FrontierMath T4 87.8%, GPQA 92.6–94.1%, Toolathlon 61.7%, GraphWalks 1M 79.4% | First GA Mythos‑class model. Fable 5 = same model with safety classifiers (falls back to Opus 4.8 on cyber/bio/distillation queries, <5% of sessions); Mythos 5 = safeguards lifted, Glasswing partners only. $10/$50. Suspended 18 days by first‑ever US export‑control order on a deployed model |
| **Claude Sonnet 5** | 2026‑06‑30 | — | — | — | 1M | C | SWE‑bench Pro 63.2% | Most agentic Sonnet; near Opus 4.8 at $2/$10 intro ($3/$15 from Sep); default model on Free/Pro |

Sources: [Anthropic news](https://www.anthropic.com/news), [Opus 4.5](https://www.anthropic.com/news/claude-opus-4-5), [Sonnet 4.5](https://www.anthropic.com/news/claude-sonnet-4-5/), [Fable 5 / Mythos 5](https://www.anthropic.com/news/claude-fable-5-mythos-5), [Redeploying Fable 5](https://www.anthropic.com/news/redeploying-fable-5), [Sonnet 5](https://www.anthropic.com/news/claude-sonnet-5), [Opus 4.1 system card](https://www.anthropic.com/claude-opus-4-1-system-card), [Models overview docs](https://docs.anthropic.com/en/docs/about-claude/models/whats-new-claude-4-5), [Artificial Analysis: Opus 4.5](https://artificialanalysis.ai/articles/claude-opus-4-5-benchmarks-and-analysis), [W&B: Opus 4.8 benchmarks](https://wandb.ai/byyoung3/ml-news/reports/Claude-Opus-4-8-Benchmark-Scores--VmlldzoxNzA0NTk3MQ), [Epoch AI](https://epoch.ai/data-insights/models-over-1e25-flop).

---

## Google / Google DeepMind

| Model | Release | Params | Compute (FLOP) | Training cost | Context | OW/C | Key benchmarks | Significance |
|---|---|---|---|---|---|---|---|---|
| **PaLM** | 2022‑04‑05 | 540B dense | ≈2.5e24 | — | 2K | C | MMLU 69.3%, GSM8K 58.1%, BIG‑bench 65% | Largest dense LM at the time; chain‑of‑thought emergence |
| **PaLM 2** | 2023‑05‑10 | "Smaller than PaLM" (rumored ~340B) | ≈1e24 | — | 8K | C | MMLU 78.3%, HumanEval 37.6% | Multilingual + code‑heavy; powered Bard |
| **Gemini 1.0 Ultra / Pro / Nano** | 2023‑12‑06 (Ultra GA 2024‑02‑08) | — | Ultra **5.0e25** (Epoch) | — | 32K | C | Ultra: MMLU 90.0% (CoT@32), MMMU 59.4%, HumanEval 74.4% | First Gemini; natively multimodal text/image/audio/video |
| **Gemini 1.5 Pro** | 2024‑02‑15 | MoE (size undisclosed) | **1.6e25** (Epoch imputed) | — | **1M → 2M** | C | MMLU ≈85%, MMMU 58.5%, near‑perfect needle‑in‑haystack at 1M | First production 1M+ context model |
| **Gemini 1.5 Flash** | 2024‑05‑14 | Smaller MoE | — | — | 1M | C | Cheap, fast | Distilled from 1.5 Pro |
| **Gemma 1 (2B/7B)** | 2024‑02‑21 | 2B / 7B | — | — | 8K | OW | Best small OW at release | Google's open‑weights line |
| **Gemma 2 (9B/27B)** | 2024‑06‑27 | 9B / 27B | — | — | 8K | OW | 27B beat Llama 3 70B on some evals | Strong dense small models |
| **Gemini 2.0 Flash** | 2024‑12‑11 (exp), GA 2025‑02‑05 | — | — | — | 1M | C | MMLU‑Pro 76.4%, MMMU 70.7% | Cheap multimodal; native tool use; Flash‑Thinking preview |
| **Gemini 2.5 Pro** (Experimental) | 2025‑03‑25 (`gemini-2.5-pro-exp-03-25`) | — | — | — | 1M (2M coming) | C | LMArena #1; AIME 2025 SOTA, GPQA Diamond 84.0%, HLE 18.8% (no tools), SWE‑bench Verified 63.8%, MMMU 81.7% | First mainline thinking‑native Gemini |
| **Gemini 2.5 Pro** (GA + Deep Think) | 2025‑05‑20 → 2025‑06 GA | — | — | — | 1M | C | + Deep Think: SOTA on USAMO 2025, LiveCodeBench, MMMU 84.0% | "Adaptive thinking" with budget control |
| **Gemini 2.5 Flash / Flash‑Lite** | 2025‑04‑17 / 2025‑06‑17 | — | — | — | 1M | C | Cost‑optimized | Wide deployment tier |
| **Gemma 3 (1B–27B)** | 2025‑03‑12 | up to 27B | — | — | 128K | OW | Best small multimodal OW at release | Multimodal Gemma |
| **Gemini 3 Pro** | 2025‑11‑18 | — | — | — | **1M in / 64K out** | C | LMArena 1501 Elo, HLE 37.5% (no tools) / 45.8% (search+code), GPQA Diamond 91.9%, ARC‑AGI‑2 31.1%, SWE‑bench Verified 76.2%, Terminal‑Bench 2.0 56.9%, MMMU‑Pro 81%, MathArena Apex 23.4%, SimpleQA Verified 72.1% | New SOTA across reasoning, coding, multimodal at release |
| **Gemini 3 Deep Think** | 2025‑11 (testers) → Ultra 2025‑Q4 | — | — | — | 1M | C | HLE 41.0% (no tools), GPQA 93.8%, ARC‑AGI‑2 45.1% | Parallel hypotheses reasoning mode |
| **Gemini 3 Flash** | 2025‑12 | — | — | — | 1M | C | Strongest Flash to date | Cheap multimodal tier |
| **Gemini 3.1 Pro** | 2026‑02‑19 | — | — | — | **1M in / 65K out** | C | HLE 44.4% (no tools) / 51.4% (search+code), **ARC‑AGI‑2 77.1%**, GPQA Diamond 94.3%, SWE‑bench Verified 80.6%, Terminal‑Bench 2.0 68.5%, LiveCodeBench Pro 2887 Elo, MathVista —, MMMU‑Pro 80.5% | Output cap raised to 65K (fixes 21K truncation in 3 Pro); current Google flagship for many tasks |
| **Gemini 3.1 Deep Think** | 2026‑02 | — | — | — | 1M | C | ARC‑AGI‑2 84.6% | Highest published ARC‑AGI‑2 score |
| **Gemini 3.5 Flash** | 2026‑05‑19 (I/O, GA same day) | — | — | — | 1M in / 65K out | C | Terminal‑Bench 2.1 76.2%, MCP Atlas 83.6%, GDPval‑AA 1656 Elo, MMMU‑Pro 83.6%, CharXiv Reasoning 84.2%, ARC‑AGI‑2 72.1% | First of the 3.5 family; beats Gemini 3.1 Pro on agentic/coding at ~4× the speed; $1.50/$9.00; default in Gemini app + AI Mode in Search; powers 24/7 personal‑agent features |
| **Gemini Omni / Omni Flash** | 2026‑05‑19 | — | — | — | — | C | Beats GPT‑5.5 / Opus 4.7 on audiovisual comprehension by 8–12pp (early reports) | Google's first natively unified any‑to‑any multimodal model (text/image/audio/video in one architecture); video generation in Gemini app, Flow, YouTube Shorts |
| **Gemma 4.5 12B** | 2026‑06‑02 | 12B | — | — | 1M | OW | Improved multimodal; audio input added | Context jump 256K → 1M native |
| **Gemini 3.5 Pro** | limited preview; GA expected mid‑July 2026 | — | — | — | 1M | C | — | Announced at I/O; still not GA as of 2026‑07‑09 |

Sources: [DeepMind Gemini page](https://www.deepmind.com/gemini), [Gemini 3 blog](https://deepmind.google/blog/a-new-era-of-intelligence-with-gemini-3/), [Gemini 3.5 blog](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5/), [Gemini 3.5 Flash API docs](https://ai.google.dev/gemini-api/docs/interactions/whats-new-gemini-3.5), [Gemini 3 Pro model card](https://deepmind.google/models/model-cards/gemini-3-pro/), [Gemini 3.1 Pro model card](https://deepmind.google/models/model-cards/gemini-3-1-pro/), [Gemini 2.5 blog](https://blog.google/technology/google-deepmind/gemini-model-thinking-updates-march-2025), [Gemini API changelog](https://ai.google.dev/gemini-api/docs/changelog), [Epoch AI](https://epoch.ai/data-insights/models-over-1e25-flop).

---

## Meta (Llama family + Muse Spark)

| Model | Release | Params | Compute (FLOP) | Training cost | Context | OW/C | Key benchmarks | Significance |
|---|---|---|---|---|---|---|---|---|
| **LLaMA 1** (7/13/33/65B) | 2023‑02‑24 | 7–65B dense | ≈1e23 (65B) | — | 2K | OW (research) | MMLU 63.4% (65B) | Sparked the open‑weights ecosystem; weights leaked |
| **Llama 2** (7/13/70B) | 2023‑07‑18 | 7–70B dense | ≈1e24 (70B) | — | 4K | OW (commercial) | MMLU 68.9%, HumanEval 29.9% (70B) | First commercially usable open frontier |
| **Llama 3** (8B/70B) | 2024‑04‑18 | 8B / 70B dense | ≈4e24 (70B est.) | — | 8K | OW | MMLU 82% (70B), HumanEval 81.7% | Best OW at release |
| **Llama 3.1** (8/70/405B) | 2024‑07‑23 | up to 405B dense | ≈4e25 (405B, Epoch) | ≈$60–100M (Meta hardware mix) | 128K | OW | 405B: MMLU 88.6%, HumanEval 89.0%, GPQA 51.1%, MATH 73.8% | First open‑weights GPT‑4‑class model |
| **Llama 3.2** (1B/3B + 11B/90B vision) | 2024‑09‑25 | 1–90B | — | — | 128K | OW | Vision MMMU ≈60% (90B) | First multimodal Llama |
| **Llama 3.3 70B** | 2024‑12‑06 | 70B | — | — | 128K | OW | Matches 3.1‑405B on most evals | Distillation gains |
| **Llama 4 Scout** (17B active / 109B total, 16 experts) | 2025‑04‑05 | 17B/109B MoE | — | — | **10M** | OW (community license) | MMLU‑Pro 74.3%, MMMU 69.4%, ChartQA 88.8% | Industry‑longest context; single H100 fit |
| **Llama 4 Maverick** (17B active / 400B total, 128 experts) | 2025‑04‑05 | 17B/400B MoE | ≈2.4M GPU‑hr | — | 1M | OW | MMLU‑Pro 80.5%, MMMU 73.4%, LiveCodeBench 43.4%, LMArena 1417 Elo (experimental chat) | Best perf/cost open MoE at release |
| **Llama 4 Behemoth** (288B active / ~2T total) | Announced 2025‑04‑05; **never released** | 288B/~2T MoE | — | — | — | Intended OW | Self‑reported preview: MATH‑500 95%, GPQA Diamond 82.2%, MMLU multilingual 85.8% | Superseded by the Llama 5 program; reportedly underperformed Gemini 2.5 Pro / Claude 4.x |
| **Llama 5 8B + Llama 5 Scout** (109B/17B active MoE) | 2026‑05‑01 | 8B dense; 109B/17B MoE | — | — | 256K | OW (Llama 5 Community License, 700M‑MAU cap) | Scout: MMLU high‑80s, native audio transcription ≈ Whisper Large v3 | Meta's open comeback after a quiet six months; first Llama with native text+vision+audio input |
| **Llama 5 70B** | 2026‑06‑04 | 70B dense | — | — | 256K | OW | MMLU 88%, HumanEval 86%, SWE‑bench Verified ≈65% | Strongest dense open model at release; multimodal; same‑day rival to Mistral Voyage Pro 70B |
| **Llama 5 405B "Frontier"** | rumored, unreleased | — | — | — | — | — | — | Larger tier teased at the Llama 5 launch event |
| **Muse Spark** | 2026‑04‑08 | undisclosed | — (claimed >10× pretraining efficiency vs Llama 4 Maverick) | — | — | **C** | MMMU Pro 80.4%, GPQA Diamond 89.5%, SWE‑bench Verified 77.4%, SWE‑bench Pro 52.4%, Terminal‑Bench 2.0 59.0, ARC‑AGI‑2 42.5%, HLE 50.2%, CharXiv Reasoning 86.4 (led all frontier), HealthBench Hard 42.8 (led) | First Meta Superintelligence Labs model and Meta's **first closed frontier release**; native multimodal with visual chain‑of‑thought; replaced Llama in the Meta AI app; ~4th place overall (AA Index 52 vs GPT‑5.4/Gemini 3.1 Pro at 57) but led on chart/medical/multimodal evals |
| **Muse Spark 1.1** | **2026‑07‑09** | undisclosed | — | — | **1M** | **C** | Terminal‑Bench 2.1 80.0 (vs 67.3 for 1.0), SWE‑bench Pro 61.5% (beats GPT‑5.5's 58.6), OSWorld‑Verified 80.8 (vs 53.3), Toolathlon‑Verified 75.6, JobBench 54.7 (led), MCP Atlas 88.1 (led), HLE w/ tools 62.1 (led), DeepSWE 1.1 53.3, GDPval‑AA v2 Elo 1381 | Big agentic/computer‑use jump in 3 months; multimodal perception+action (video/image/audio in long agentic workflows, visual‑to‑code, ultra‑descriptive captioning); multi‑agent orchestration (main agent delegates to parallel subagents); launched the paid **Meta Model API** (public preview, $1.25/$4.25 per Mtok) — Meta now sells closed model access like OpenAI/Anthropic |

Sources: [Meta Llama 4 launch blog](https://ai.meta.com/blog/llama-4-multimodal-intelligence), [Llama 4 product page](https://www.llama.com/models/llama-4/), [LLMCheck May 2026 open‑source recap](https://llmcheck.net/blog/state-of-open-source-local-llms-may-2026/), [LLMCheck June 2026 recap](https://llmcheck.net/blog/state-of-open-source-local-llms-june-2026/), [Epoch AI](https://epoch.ai/data-insights/models-over-1e25-flop), [Muse Spark launch](https://ai.meta.com/blog/introducing-muse-spark-msl/), [Muse Spark 1.1 + Meta Model API](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/), [DataCamp Muse Spark 1.1 analysis](https://www.datacamp.com/blog/muse-spark-1-1).

---

## DeepSeek

| Model | Release | Params | Compute (FLOP) | Training cost | Context | OW/C | Key benchmarks | Significance |
|---|---|---|---|---|---|---|---|---|
| **DeepSeek‑V2** | 2024‑05 | 236B/21B active MoE | ≈1e24 | — | 128K | OW | MMLU 78.5%, HumanEval 81.1% | Pioneered MLA + DeepSeekMoE |
| **DeepSeek‑V3** | 2024‑12‑26 | 671B/37B active MoE | ≈3.4e24 (2.79M H800‑hours) | ≈**$5.58M** (paper) | 128K | OW (MIT) | MMLU 88.5%, HumanEval 82.6%, MATH 90.2%, GPQA 59.1%, LiveCodeBench 40.5%, SWE‑bench 42.0% | Frontier‑class OW at <$6M training; market shock |
| **DeepSeek‑V3‑0324** | 2025‑03‑24 | 671B/37B | — | — | 128K | OW | Beats GPT‑4.5 on math/coding (per DeepSeek) | Quietly pushed; lessons from R1 RL |
| **DeepSeek‑R1‑Zero / R1** | 2025‑01‑20 | 671B/37B MoE | RL phase: 80h × 512 H800 → ≈**$294K** RL (Nature) | Cumulative w/ V3 base ≈$5.87M | 128K | OW (MIT) | AIME 2024 79.8%, MATH‑500 97.3%, MMLU 90.8%, GPQA Diamond 71.5%, LiveCodeBench 65.9%, SWE‑bench Verified 49.2%, Codeforces 2029 | First OW model at o1 level; pure‑RL reasoning |
| **DeepSeek‑R1‑0528** | 2025‑05‑28 | 671B/37B | — | — | 128K | OW | AIME 2024 ≈87% | Improved R1 |
| **DeepSeek‑V3.1** | 2025‑08‑21 | 671B/37B | — | — | 128K | OW | Hybrid reason/non‑reason in one model; chain‑of‑thought 20–50% shorter than R1‑0528 at parity | First hybrid reasoning OW; trained for upcoming domestic chips |
| **DeepSeek‑V3.1‑Terminus** | 2025‑09‑22 | 671B/37B | — | — | 128K | OW | Stability fixes | Minor refresh |
| **DeepSeek‑V3.2‑Exp** | 2025‑09‑29 | 671B/37B | — | — | 128K | OW | At parity w/ V3.1‑Terminus | Introduced **DeepSeek Sparse Attention** |
| **DeepSeek‑V3.2 / V3.2‑Speciale** | 2025‑12‑01 | 671B/37B | — | — | 128K | OW (V3.2); API‑only (Speciale) | V3.2: AIME 2025 93.1%, GPQA Diamond 82.4%, LiveCodeBench v6 83.3%, HLE 25.1%; **Speciale**: AIME 96.0%, HMMT Feb 2025 99.2%, Codeforces 2701, GPQA 85.7%, HLE 30.6%, gold‑medal IMO/CMO/IOI/ICPC 2025 | Speciale rivals Gemini 3 Pro / GPT‑5 on reasoning |
| **DeepSeek‑V4 Pro** | 2026‑04‑24 (preview; official release due mid‑July 2026) | **1.6T total / 49B active** MoE | — | — | **1M (native)** | OW (MIT) | SWE‑bench Verified 80.6%, LiveCodeBench 93.5%, Codeforces 3206, HLE 37.7%, GPQA Diamond 90.1%, HMMT 2026 95.2%; SimpleQA‑Verified ≈+20pp over other OSS | Production‑viable ultra‑long context (27% FLOPs / 10% KV cache vs V3.2 at 1M); thinking now a per‑request setting (`thinking: off/on/max`) |
| **DeepSeek‑V4 Flash** | 2026‑04‑24 | 284B / 13B active MoE | — | — | 1M | OW (MIT) | SWE‑bench Verified ≈79% | Cost‑efficient sibling ($0.14/$0.28 per Mtok); many production stacks route cheap traffic here |

Note: DeepSeek never shipped a model branded "R2" (still true as of July 2026 — Reuters reported Liang Wenfeng held it back over performance; some third‑party "R2 launch" posts in May 2026 are unreliable). V3.1 unified reasoning + non‑reasoning into one model, and the reasoning frontier is carried by V4‑Pro thinking mode. The hosted R1 endpoint retires July 24, 2026.

Sources: [DeepSeek API change log](https://api-docs.deepseek.com/updates/), [BentoML DeepSeek guide (2026)](https://www.bentoml.com/blog/the-complete-guide-to-deepseek-models-from-v3-to-r1-and-beyond), [DeepSeek‑V3.2 paper (arXiv 2512.02556)](https://arxiv.org/html/2512.02556v1), [V3.2 release notes](https://api-docs.deepseek.com/news/news251201), [Reuters on R1 cost](https://www.reuters.com/world/china/chinas-deepseek-says-its-hit-ai-model-cost-just-294000-train-2025-09-18/), [The Register on full cost](https://www.theregister.com/2025/09/19/deepseek_cost_train/).

---

## xAI / SpaceXAI

Corporate note: SpaceX absorbed xAI in a February 2026 all‑stock deal (~$1.25T combined) and rebranded the unit **SpaceXAI** in May 2026. SpaceX IPO'd on Nasdaq June 12 ($75B raised, largest ever) and agreed June 16 to acquire Anysphere (Cursor) for $60B. Grok 5 (reportedly 6T‑parameter MoE) remains in training on Colossus 2 as of July 2026, having missed Q1 and Q2 targets.

| Model | Release | Params | Compute (FLOP) | Training cost | Context | OW/C | Key benchmarks | Significance |
|---|---|---|---|---|---|---|---|---|
| **Grok 1** | 2023‑11‑04 (xAI), weights 2024‑03‑17 | 314B MoE (8 experts, ~86B active) | — | — | 8K | OW (Apache 2.0, base only) | MMLU 73%, HumanEval 63.2% | First xAI model; large open MoE |
| **Grok 1.5** | 2024‑03‑28 | — | — | — | 128K | C | MATH 50.6%, HumanEval 74.1%, MMLU ≈81% | Long context |
| **Grok 1.5V** | 2024‑04 | — | — | — | 128K | C | First multimodal Grok | Vision |
| **Grok 2** | 2024‑08‑13 | — | — | — | 128K | C | MMLU‑Pro 75.5%, MATH 76.1%, HumanEval 88.4%, GPQA 56.0% | Trained on Memphis "Colossus" cluster ramp |
| **Grok 3** | 2025‑02‑17 | — | ≈10× Grok 2 (xAI claim) | — | 128K | C | AIME 2025 93.3% (think), MATH ≈98%, GPQA 84.6% | First version with "Think" + "DeepSearch" |
| **Grok 4 / Grok 4 Heavy** | 2025‑07‑09 | Undisclosed (≈1.7T per third‑party leak; unverified) | Trained on **200K H100 Colossus cluster**, 6× efficiency, "order of magnitude more compute than Grok 3" | — | 256K (API) / 1M (app), 128K out | C | **HLE 50.7%** (Heavy, text+tools — first model >50%), GPQA Diamond 87.5–88.4%, AIME 2025 91.7% (100% Heavy), USAMO 2025 61.9%, ARC‑AGI‑2 15.9%, LiveCodeBench 79%, Vending‑Bench $4694 net | First model to break 50% on HLE; native tool use baked into RL |
| **Grok 4.1** | 2025‑Q3 | — | — | — | 256K | C | Personality + reasoning refresh | Minor update |
| **Grok 4 Fast** | 2025‑Q4 | — | — | — | 2M | C | Cheap reasoner ($0.20/$0.50 per Mtok) | Long context tier |
| **Grok 4.20 / 4.20 Beta 2** | 2026‑03 | — | — | — | — | C | Per IBTimes Australia: top medical/legal/general benchmark leaderboards in April 2026 | 4‑agent system; 83% non‑hallucination rate |
| **Grok 4.3** | 2026‑04‑17 (beta) → ~04‑30 GA | ≈0.5T (Musk‑confirmed) | — | — | 2M | C | Leading agentic tool‑calling / instruction‑following per third parties | Unified flagship: all prior API slugs retired to `grok-4.3` on May 15 at $1.25/$2.50 per Mtok; native video understanding |
| **Grok 4 Open** | 2026‑06‑05 | 100B / 20B active MoE | — | — | 128K | OW ("xAI Custom License" — attribution + no‑competing‑model clauses; not OSI) | MMLU 86%, SWE‑bench Verified 69%, AIME 2025 82%, integrated tool use 93% | xAI's **first‑ever open‑weights release**; 1.4M downloads in 48h |
| **Grok 4.5** | 2026‑07‑08 | Built on "V9" 1.5T foundation (reported) | — | — | — | C | SWE‑bench Pro 64.7%, Terminal‑Bench 2.1 83.3%, SWE Marathon 29.0% (beats Fable 5 + Opus 4.8), DeepSWE 62.0% | "Opus‑class but faster/cheaper" (Musk): $2/$6, ~80 TPS, ~2× token efficiency (15,954 avg output tokens/SWE‑bench‑Pro task vs 67,020 for Opus 4.8 max); trained alongside Cursor; not yet EU‑available |

Sources: [Grok 4 announcement](https://x.ai/news/grok-4), [Grok 4.5 announcement](https://x.ai/news/grok-4-5), [Awesome Agents: Grok 4.3](https://awesomeagents.ai/models/grok-4-3/), [SQ Magazine on Grok 4.5](https://sqmagazine.co.uk/grok-4-5-launch/), [LLMCheck June 2026 (Grok 4 Open)](https://llmcheck.net/blog/state-of-open-source-local-llms-june-2026/), [IBTimes AU on Grok 4.20 Beta 2](https://www.ibtimes.com.au/grok-420-beta-2-powers-xai-advances-model-tops-benchmarks-saves-lives-april-2026-1866556).

---

## Alibaba (Qwen)

| Model | Release | Params | Compute (FLOP) | Training cost | Context | OW/C | Key benchmarks | Significance |
|---|---|---|---|---|---|---|---|---|
| **Qwen 1 / 1.5** | 2023‑08 → 2024‑02 | 0.5–72B | — | — | 32K | OW (Apache‑2.0 partial) | MMLU 77.4% (72B) | First widely used Qwen |
| **Qwen 2** | 2024‑06‑07 | 0.5–72B | — | — | 128K | OW | MMLU 84.2% (72B) | Strong open multilingual |
| **Qwen 2.5 / 2.5‑Max** | 2024‑09‑19 / 2025‑01‑29 | up to 72B; Max MoE (size undisclosed) | — | — | 128K | OW (≤72B); Max C | MMLU‑Pro 76.1%, GPQA 49.0% (72B); Max ≈ Claude 3.5 | 2.5‑Max API was Alibaba's first frontier‑class API |
| **QwQ‑32B / QwQ‑Max** | 2024‑11‑27 / 2025‑02‑25 | 32B dense | — | — | 32K | OW | AIME 50%, GPQA 65% (32B) | First open reasoning model from Alibaba |
| **Qwen 3 (0.5B–235B MoE)** | 2025‑04‑29 | up to 235B/22B active | — | — | 128K | OW (Apache‑2.0) | MMLU‑Pro 82%, AIME 2025 81%, LiveCodeBench 65% (235B) | Hybrid thinking/non‑thinking, fully OSS |
| **Qwen3‑Max** | 2025‑09‑05 | 1T+ MoE | — | — | 262K | C | MMLU‑Pro 81%, SWE‑bench Verified 69.6%, AIME 2025 high | Alibaba's first trillion‑parameter flagship; pre‑trained on 36T tokens |
| **Qwen3‑Max‑Thinking** (`qwen3-max-2026-01-23`) | 2026‑01‑27 | 1T+ MoE | — | — | 262K | C | GPQA Diamond 92.8, AIME 2025 100% (Heavy TTS), HLE w/ search 58.3, LiveCodeBench v6 91.4, IMO‑AnswerBench 91.5, SWE‑bench Verified 75.3 | Adaptive tool use + multi‑round test‑time scaling; ties/leads frontier on math+search |
| **Qwen3.5 (open, 397B MoE)** | 2026‑02‑16 | 397B/A17B MoE | — | — | 256K | OW (Apache‑2.0) | Highest open generalist at release | New GatedDeltaNet hybrid architecture |
| **Qwen3.5‑Max‑Preview** | 2026‑03‑19 (LMArena debut) | unknown | — | — | 256K+ | C (preview) | LMArena rank #10 English; beats GPT‑5.4, Claude 4.5 Opus on prompts; AIME 2026 91.3, GPQA Diamond 88.4, LiveCodeBench v6 83.6, SWE‑bench Verified 76.4, MMLU‑Pro 87.8, MathVista 90.3 | New native multimodal architecture; API expected Q2 2026 |
| **Qwen3.6‑27B** | 2026‑04‑22 | 27B dense | — | — | 256K+ | OW (Apache‑2.0) | SWE‑bench Verified 77.2%, SWE‑bench Pro 53.5%, Terminal‑Bench 2.0 59.3%, GPQA Diamond 87.8% | Dense model beats own 397B MoE on agentic coding; hybrid GatedDeltaNet/self‑attn |
| **Qwen 3.7 Max** | 2026‑05‑20 | — | — | — | 256K+ | C (API) | SWE‑bench Pro 60.6%, Terminal‑Bench 2.0 69.7%, GPQA 92.4% | "The Agent Frontier" flagship; $2.50/$7.50 per Mtok |
| **Qwen 4** (32B‑A3B, Preview 05‑05 → full 06‑01) | 2026‑06‑01 | 32B / 3B active MoE (128 experts) | — | — | **1M native** | OW (Apache‑2.0) | SWE‑bench Verified 78%, MMLU 89%, HumanEval 94%, AIME 2025 91% | New #1 open model runnable on consumer hardware (24GB); trained on 20T tokens; hybrid auto reasoning |
| **Qwen 4 Coder 32B‑A3B** | 2026‑06‑02 | 32B/3B MoE | — | — | 256K | OW (Apache‑2.0) | **SWE‑bench Verified 82%**, HumanEval 96%, LiveCodeBench 78–79% | First permissively‑licensed consumer‑runnable coder above 80% SWE‑V; post‑trained on ~4T extra code/agentic tokens |
| **Qwen 4 4B** | 2026‑06‑03 | 4B | — | — | 256K | OW (Apache‑2.0) | MMLU 84% | Best 8GB‑tier model; 135 tok/s on laptop hardware |

Sources: [Qwen3‑Max overview (qwen-ai.com)](https://qwen-ai.com/qwen-max/), [Alibaba Cloud blog: Qwen3‑Max‑Thinking](http://www.alibabacloud.com/blog/pushing-qwen3-max-thinking-beyond-its-limits_602834), [Alibaba Cloud: Qwen3.6‑27B](https://www.alibabacloud.com/blog/qwen3-6-27b-flagship-level-coding-in-a-27b-dense-model_603063), [LLMCheck June 2026 (Qwen 4)](https://llmcheck.net/blog/state-of-open-source-local-llms-june-2026/), [MarkTechPost: Qwen3.6‑27B](https://www.marktechpost.com/2026/04/22/alibaba-qwen-team-releases-qwen3-6-27b-a-dense-open-weight-model-outperforming-397b-moe-on-agentic-coding-benchmarks/).

---

## Mistral

| Model | Release | Params | Compute (FLOP) | Training cost | Context | OW/C | Key benchmarks | Significance |
|---|---|---|---|---|---|---|---|---|
| **Mistral 7B** | 2023‑09‑27 | 7B dense | — | — | 8K | OW (Apache‑2.0) | MMLU 60.1%, HumanEval 30% | Best 7B at release; SWA + GQA |
| **Mixtral 8×7B** | 2023‑12‑11 | 47B (12.9B active) MoE | — | — | 32K | OW | MMLU 70.6%, HumanEval 40.2% | Popularized open MoE |
| **Mistral Large 1** | 2024‑02‑26 | undisclosed dense | — | — | 32K | C | MMLU 81.2%, HumanEval 45% | First Mistral closed flagship |
| **Mixtral 8×22B** | 2024‑04‑10 | 141B (39B active) MoE | — | — | 64K | OW | MMLU 77.7%, HumanEval 76.5% | Strong open MoE |
| **Mistral Large 2** (`24.07`) | 2024‑07‑24 | 123B dense | — | — | 128K | OW (research; commercial via API) | MMLU 84.0%, HumanEval ≈92%, MATH ≈58% | Near‑GPT‑4o on coding/math; multilingual |
| **Mistral Small 3 / Codestral 25.01** | 2025‑01–03 | 24B / Codestral | — | — | 128K | OW / C | Strong code | Cost‑efficient open small + new Codestral |
| **Mistral Medium 3** | 2025‑05‑07 | undisclosed | — | — | 128K | C | At/above 90% of Claude 3.7 Sonnet at 8× lower cost; beats Llama 4 Maverick / Command A | Frontier perf at $0.40/$2.00 per Mtok |
| **Mistral Large 3** | 2025‑12‑02 | **675B / 41B active** MoE, multimodal | — | — | 256K | OW (Apache‑2.0) | MMLU‑Pro 73.1%, MATH‑500 93.6%, HumanEval 90.2%, AIME 2025 40.0%, GPQA 43.9% (no thinking), Terminal‑Bench 23.75% | Largest fully Apache‑2.0 model at release |
| **Mistral Medium 3.5** | 2026‑04 (late) | — | — | — | 256K | OW (Apache‑2.0) | SWE‑bench Verified 77.6% | The "EU‑jurisdiction frontier" pick under GDPR/AI Act procurement |
| **Mistral Voyage 24B** | 2026‑05‑03 | 24B dense | — | — | 256K | OW (Apache‑2.0) | Strong mid‑size generalist | New "Voyage" line |
| **Mistral Voyage Pro 70B** | 2026‑06‑04 | 70B dense | — | — | 512K | OW (Apache‑2.0) | SWE‑bench Verified 68%, tool‑use accuracy 91%, MMLU 85% | Apache‑2.0 70B released same day as Llama 5 70B; the license‑friendly agentic pick |

Sources: [Mistral Large 2 announcement](https://mistral.ai/fr/news/mistral-large-2407), [Mistral Medium 3 announcement](https://mistral.ai/news/mistral-medium-3), [LayerLens: Mistral Large 3](https://medium.com/@layerlens/mistral-large-3-early-results-from-atlas-13f6a3c6b35a), [LLMCheck June 2026 (Voyage Pro)](https://llmcheck.net/blog/state-of-open-source-local-llms-june-2026/), [jamesm.blog: open‑weight state 2026](https://jamesm.blog/ai/state-of-open-weight-models-2026/).

---

## Moonshot AI (Kimi)

| Model | Release | Params | Compute (FLOP) | Training cost | Context | OW/C | Key benchmarks | Significance |
|---|---|---|---|---|---|---|---|---|
| **Kimi K2** (Base + Instruct) | 2025‑07‑15 | **1T total / 32B active** MoE (384 experts, 8 active) | — | — | 128K | OW (Modified MIT) | MMLU 87.8, GPQA‑Diamond 48.1, LiveCodeBench v6 26.3, SWE‑bench Verified 65.8 (single) / 71.6 (multi), MATH 70.2, MATH‑500 97.4 | First OW 1T MoE; agentic + tool use focus; MuonClip optimizer |
| **Kimi K2‑Instruct‑0905** | 2025‑09 | 1T/32B | — | — | 128K | OW | SWE‑bench Verified 69.2 | Iterative improvement |
| **Kimi K2 Thinking** | 2025‑11‑06 | 1T/32B | — | — | 128K | OW (Mod. MIT) | **HLE 44.9%, BrowseComp 60.2%, SWE‑bench Verified 71.3%, LiveCodeBench v6 83.1%, GPQA 85.7%, Seal‑0 56.3%** | First OW model to exceed GPT‑5 + Claude Sonnet 4.5 on agentic evals |
| **Kimi K2.5** | 2026‑01 | 1T/32B | — | — | 128K | OW | Multimodal + Agent Swarm v1 | Multimodal + multi‑agent |
| **Kimi K2.6** (GA) | 2026‑04‑21 (Code Preview 04‑13) | 1T/32B (384 experts) | — | — | 256K | OW (Mod. MIT) | Terminal‑Bench 2.0 66.7%, SWE‑bench Pro 58.6%, SWE‑bench Verified 80.2%, MathVision (w/ Python) 93.2% | 12‑hour coding runs; up to 300 sub‑agents/swarm, 4,000+ tool calls; native INT4 QAT |
| **Kimi K2.7‑Code** | 2026‑06‑12 | 1T/32B MoE + 400M MoonViT vision encoder | — | — | 256K | OW (Mod. MIT) | Coding‑focused build on K2.6 | Coding specialist; K2.6 remains the general agent‑swarm pick |

Sources: [VentureBeat on K2 Thinking](https://venturebeat.com/ai/moonshots-kimi-k2-thinking-emerges-as-leading-open-source-ai-outperforming), [K2 Thinking blog](https://kimi-k2.org/blog/15-kimi-k2-thinking-en), [K2.6 release](https://kimi-k2.org/blog/24-kimi-k2-6-release), [GitHub: moonshotai/Kimi-K2](https://github.com/moonshotai/kimi-K2), [Spectrum AI Lab: open models 2026](https://spectrumailab.com/blog/best-open-source-ai-models-ranked-2026), [AINews on K2 launch](https://www.ainews.com/p/moonshot-ai-releases-kimi-k2-a-1t-open-source-model-built-for-agentic-reasoning).

---

## Other notable releases

| Model | Release | Developer | Params | Context | OW/C | Significance |
|---|---|---|---|---|---|---|
| **Cohere Command R / R+** | 2024‑03 / 2024‑04 | Cohere | 35B / 104B | 128K | OW (research) | RAG/tool‑use specialty |
| **Cohere Command A** | 2025‑03 | Cohere | 111B | 256K | OW (research) | Enterprise RAG flagship |
| **Phi‑3 (mini/small/medium)** | 2024‑04 | Microsoft | 3.8B–14B | 128K | OW (MIT) | Tiny‑model "data‑quality" approach |
| **Phi‑4 / Phi‑4‑reasoning** | 2024‑12 / 2025‑05 | Microsoft | 14B | 16K | OW | Strong small reasoning |
| **Inflection‑2.5** | 2024‑03 | Inflection | undisclosed | — | C | "40% of GPT‑4 compute"; ≈1e25 FLOP (Epoch) |
| **Reka Core** | 2024‑04 | Reka AI | undisclosed | 128K | C | Multimodal ≈ GPT‑4 class |
| **Falcon 180B** | 2023‑09 | TII (UAE) | 180B dense | 8K | OW | Largest OW at release; ≈3.8e24 FLOP (Epoch) |
| **Yi‑Large / Yi‑1.5** | 2024‑05 | 01.AI | 34B / unspecified large | 200K (Yi‑1.5) | OW | Top Chinese OW in 2024 |
| **GLM‑4 / GLM‑4‑Plus** | 2024‑01 / 2024‑08 | Zhipu AI | undisclosed | 128K | C | Chinese frontier; **GLM‑4‑Plus 3.6e25 FLOP** (Epoch) |
| **Doubao‑pro** | 2024 | ByteDance | undisclosed | — | C | **2.5e25 FLOP** (Epoch); main model behind Doubao chatbot |
| **GPT‑OSS 120B / 20B** | 2025‑08‑05 | OpenAI | 120B / 20B (MoE) | 128K | OW (Apache‑2.0) | OpenAI's first OSS reasoning models since GPT‑2 |
| **MiniMax‑M2** | 2025‑10 | MiniMax | undisclosed MoE | 200K+ | OW | Briefly "king of OSS"; eclipsed by Kimi K2 Thinking weeks later |
| **MiniMax‑M3** | 2026‑H1 | MiniMax | undisclosed MoE | 200K+ | OW | SWE‑bench Pro 59.0% at $2.40/M output — top open perf/cost |
| **GLM‑5.2** | 2026‑H1 | Zhipu / Z.ai | undisclosed MoE | 200K | OW | SWE‑bench Pro 62.1% — strongest open coding model on that board |
| **Phi‑5 Mini / Medium 14B** | 2026‑05 / 2026‑05‑30 | Microsoft | 4B / 14B | 64K→256K | OW (MIT) | Medium: MMLU 86%, AIME 2025 75% — GPT‑4‑class at 14B |
| **Stripe of Chinese OW frontier**: Yi, GLM, Doubao, Qwen, DeepSeek, Kimi, MiniMax | 2024–2026 | various | various | — | mostly OW | Closed the gap with US frontier in 2025–2026 |

---

## Key takeaways

1. **Compute scaling continued**: From GPT‑3 (~3e23 FLOP) to GPT‑4 (2.1e25) to GPT‑4.5 (6.4e25) and clearly past 1e26 for GPT‑5/Gemini 3 (numbers undisclosed but inferable from cluster size and training duration). Epoch AI tracked >30 models above 1e25 FLOP by mid‑2025.
2. **Costs flattened from the developer's perspective**: DeepSeek V3 was trained for ~$5.6M (Dec 2024) and matched many Western frontier models. Anthropic confirmed Claude 3.5 Sonnet and 3.7 Sonnet each cost "tens of millions" — far below the rumored hundreds of millions for GPT‑4.5. Frontier *capabilities* are getting cheaper to reproduce even as raw frontier *compute* keeps climbing.
3. **The reasoning paradigm shift** (Sep 2024 → present): o1‑preview kicked off explicit "thinking" models. By 2026 every frontier vendor ships hybrid (instant + thinking + pro) models with parallel test‑time compute — and mid‑2026 pushed it further into **multi‑agent test‑time compute** (GPT‑5.6 `ultra` coordinating 4–16 parallel agents, Claude Dynamic Workflows with hundreds of subagents, Kimi K2.6 300‑agent swarms).
4. **Benchmark saturation**: MMLU and HumanEval are saturated; the relevant frontier evals in mid‑2026 are SWE‑bench Pro, Terminal‑Bench 2.1, ARC‑AGI‑2/3, GPQA Diamond, Humanity's Last Exam, FrontierMath, BrowseComp, OSWorld 2.0, GDPval / Agents' Last Exam, and long‑horizon agentic tracks (SWE Marathon, DeepSWE).
5. **Open weights closed most of the gap** in 2025–2026. By mid‑2026 the open Pareto frontier (DeepSeek V4 Pro, Kimi K2.6/K2.7, Qwen 4, GLM‑5.2, Llama 5 70B, Mistral Voyage Pro) is within a few percentage points of the closed frontier on most coding and reasoning benchmarks — and in the May–June 2026 wave, **every major Western lab except Anthropic and OpenAI shipped downloadable weights** (Meta Llama 5, Mistral Voyage, Google Gemma 4.5, Microsoft Phi‑5, and even xAI's Grok 4 Open). At the same time the open‑weights champion went dual‑track: Meta's frontier line (Muse Spark, closed, paid API as of July) now sits *above* its open Llama line.
6. **Context windows exploded**: from 4K (2022) → 128K (2023) → 1M (Gemini 1.5, 2024) → 10M (Llama 4 Scout, 2025) → native 1M as table stakes even for open models (DeepSeek V4, Qwen 4, Gemma 4.5, Claude 4.6+, Gemini 3.x).
7. **Government entered the release loop** (new in 2026): Anthropic's Fable 5 / Mythos 5 were suspended for 18 days under a first‑of‑its‑kind US export‑control directive (June 12–30), and OpenAI's GPT‑5.6 launched first as a government‑coordinated limited preview. Frontier cyber capability (ExploitBench, Mythos‑class hacking skills) is now a deployment gate, with "trusted access" programs (Project Glasswing, OpenAI Daybreak) becoming the pattern.

---

## Primary sources

- [Epoch AI — Notable AI Models database](https://epoch.ai/data/ai-models)
- [Epoch AI — >1e25 FLOP tracker (June 2025)](https://epoch.ai/data-insights/models-over-1e25-flop)
- [Epoch AI — Tracking large‑scale AI models](https://epoch.ai/blog/tracking-compute-intensive-ai-models)
- OpenAI: [Release notes](https://help.openai.com/en/articles/6825453-chatgpt-release-notes), [GPT‑5](https://openai.com/index/introducing-gpt-5/), [GPT‑5.2](https://openai.com/index/introducing-gpt-5-2/)
- Anthropic: [News index](https://www.anthropic.com/news), [Models docs](https://docs.anthropic.com/en/docs/about-claude/models/whats-new-claude-4-5)
- Google DeepMind: [Gemini 3](https://deepmind.google/blog/a-new-era-of-intelligence-with-gemini-3/), [model cards](https://deepmind.google/models/), [Gemini API changelog](https://ai.google.dev/gemini-api/docs/changelog)
- Meta: [Llama 4 launch](https://ai.meta.com/blog/llama-4-multimodal-intelligence)
- DeepSeek: [API change log](https://api-docs.deepseek.com/updates/), [V3.2 paper (arXiv 2512.02556)](https://arxiv.org/html/2512.02556v1), [BentoML guide](https://www.bentoml.com/blog/the-complete-guide-to-deepseek-models-from-v3-to-r1-and-beyond)
- xAI: [Grok 4](https://x.ai/news/grok-4)
- Alibaba: [Qwen3‑Max‑Thinking blog](http://www.alibabacloud.com/blog/pushing-qwen3-max-thinking-beyond-its-limits_602834)
- Mistral: [Large 2](https://mistral.ai/fr/news/mistral-large-2407), [Medium 3](https://mistral.ai/news/mistral-medium-3)
- Moonshot AI: [Kimi K2 Thinking blog](https://kimi-k2.org/blog/15-kimi-k2-thinking-en)
- Independent benchmark services: [Artificial Analysis](https://artificialanalysis.ai/), [LMArena](https://lmarena.ai/), [ARC Prize](https://arcprize.org/), [Vellum benchmarks](https://www.vellum.ai/blog/), [APXML](https://apxml.com/), [DocsBot](https://docsbot.ai/)

_Compiled April 26, 2026; updated July 9, 2026 (May–July release wave: Llama 5, Gemini 3.5 Flash/Omni, Opus 4.8, Fable/Mythos 5, Sonnet 5, Qwen 4, Grok 4 Open/4.5, GPT‑5.6). Treat all undisclosed compute, parameter, and cost figures as approximate; mark them as such when citing._
