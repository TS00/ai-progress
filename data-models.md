# Frontier AI/LLM Model Releases — June 2020 to September 2026

A structured, sourced compilation of significant frontier model releases from GPT‑3 through September 23, 2026.

## Methodology and caveats

- **Scope**: "frontier" releases only — models that set or contested state of the art at release, plus the most influential open‑weights drops. Minor checkpoints (e.g., dated revisions, mini/nano variants) are noted in the parent row rather than given their own entry, except where they had distinct strategic importance.
- **Compute (FLOP)** and **training cost (USD)** for closed models are almost never officially disclosed. Numbers come primarily from the [Epoch AI Notable AI Models database](https://epoch.ai/data/ai-models) and their [>1e25 FLOP tracker](https://epoch.ai/data-insights/models-over-1e25-flop). Most are imputed from benchmarks or estimated from hardware × duration; treat them as **order‑of‑magnitude estimates**.
- **Parameter counts** for closed models are unconfirmed unless sourced from the developer. Where third‑party leaks are the only source, they are flagged as such.
- **Benchmarks** are reported as the developer or independent evaluator stated them at release. Different harnesses, prompt scaffolds, tool budgets, and "thinking" modes are not directly comparable across rows; numbers are indicative, not definitive. Where multiple modes exist (e.g. "high"/"thinking"/"pro"), the strongest publicly reported number is shown.
- "OW" = open‑weights, "C" = closed.
- "≈" = approximate, "—" = not disclosed / not applicable / no comparable benchmark at the time.
- Today's date: **September 23, 2026**.

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
| 2026‑07 | Kimi K3 (2.8T) | Moonshot AI | Largest open‑weights model ever (2.8T/104B); #4 overall on AA Index; US distillation accusation |
| 2026‑07 | Gemini 3.6 Flash + 3.5 Flash Cyber | Google DeepMind | Monthly Flash cadence begins; Gemini 4 pre‑training confirmed same day |
| 2026‑07 | Claude Opus 5 | Anthropic | New general‑purpose flagship; near‑Fable‑5 intelligence at half the price |
| 2026‑07 | DeepSeek V4‑Flash‑0731 | DeepSeek | Official Flash release; MIT weights; agent re‑post‑train at $0.14/$0.28 |
| 2026‑08 | OpenAI names **Astra** | OpenAI | Ten new machine‑checked math/TCS results (Aug 1); first‑ever "Critical" cyber designation (Aug 7); unreleased |
| 2026‑08 | Qwen3.8‑Max (2.4T) | Alibaba | First Max‑class flagship with open weights (checkpoint Aug 12) |
| 2026‑08 | Muse Spark 1.2 + Muse Code | Meta (MSL) | Meta's first coding agent; model + harness co‑trained; contributor (data‑for‑discount) tier |
| 2026‑08 | Grok 4.6 | xAI/SpaceXAI | GPQA Diamond 94.9% record; AA Index 61 ties GPT‑5.6 Sol max; Cursor deal closes 2 days later |
| 2026‑08 | DeepSeek V4‑Pro‑0813 GA | DeepSeek | 1.6T flagship GA; first peak/off‑peak API pricing — end of the subsidized‑inference era |
| 2026‑08 | GLM‑5.3 | Zhipu / Z.ai | Post‑training‑only upgrade tops GDPval‑AA v2 (1769 Elo) at launch; open‑source SOTA on Terminal‑Bench 3.0 until V4.1‑Flash |
| 2026‑09 | Claude Fable 5.1 / Mythos 5.1 | Anthropic | Same weights; Fable GA, Mythos trusted‑access. Leads AA Index v4.1.1 (65.7) and HLE with tools (65.0%) |
| 2026‑09 | Gemini 3.8 Flash + Flash Cyber | Google DeepMind | Third Flash in six weeks; Fairwind cyber program. Weak on Terminal‑Bench 4.0 (19.1%) |
| 2026‑09 | Muse Spark 1.3 | Meta (MSL) | Long‑horizon agent post‑train; ~20% fewer tool calls than 1.2 |
| 2026‑09 | GPT‑6 Astra | OpenAI | The August "Astra" name, shipped. Critical cyber confirmed. ARC‑AGI‑3 99.9%, FrontierMath T4 97.6% |
| 2026‑09 | DeepSeek V4.1‑Flash | DeepSeek | New Causal Encoder–Decoder (552B, 8B/16B active). Beats and then replaces V4‑Pro on the API |
| 2026‑09 | Grok 4.7 | xAI/SpaceXAI | New larger base than 4.6; same $2/$6 |

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

| **GPT‑6 Astra** | Named 2026‑08‑01; limited preview **2026‑09‑03**; paid GA **2026‑09‑04** | — | New pretraining run. Aidan Clark (VP of research) told Fortune it was the first OpenAI pretrain on **more than 100,000 GPUs**, at Stargate in Texas | — | **1.05M** in / 128K out (API); knowledge cutoff Apr 30, 2026 | C | OpenAI launch table: **ARC‑AGI‑3 99.9%** (Sol 7.8%), **FrontierMath T4 v2 97.6%** (lede rounds to 98%), **ExploitBench 100%** (Sol 78.5%), GPQA Diamond 96.0%, Terminal‑Bench 4.0 57.9%, Terminal‑Bench Science 0.1 64.6%, ARC‑AGI‑2 95.0%, OSWorld 2.0 72.6%, DeepSWE v1.1 74.1%, Agents' Last Exam 59.3%, ScreenSpot‑Pro 92.7%, SRE‑Bench 88.0%, HLE with tools **57.2%** (trails Fable 5.1's 65.0% in the same table). AA Intelligence Index **v4.1.1: 61.2** (Fable 5.1 65.7, Opus 5 63.1, Fable 5 62.1, Sol 60.9). AA Coding Agent Index v1.4: 67.0 (Opus 5 leads at 68.1) | The August research model, shipped as the first GPT‑6. Confirmed at the **Critical** cyber threshold; the public model refuses some cyber prompts. During eval (no production safeguards) it found two previously unknown zero‑days. Aug 1 post still stands: ten new machine‑checked math/TCS results. Press reports (Fortune, The Information, TechCrunch) say training used a recurrent‑depth / looped‑transformer technique that can obscure chain‑of‑thought. $10/$50 per Mtok; fast mode is 2× speed at 2× price. Enterprise access off by default |

Notes: OpenAI's June 26 preview marked a new deployment pattern — at the US government's request GPT‑5.6 launched first to a small set of vetted partners (citing frontier cyber capability: ExploitBench 73.5% vs GPT‑5.5's 47.9%), with GA following two weeks later alongside a hardware‑passkey "Trusted Access for Cyber" program. In late July OpenAI cut GPT‑5.6 Terra to $2/$12 and Luna to $0.20/$1.20 per Mtok; Sol stayed at $5/$30.

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
| **Claude Sonnet 5** | 2026‑06‑30 | — | — | — | 1M | C | SWE‑bench Pro 63.2% | Most agentic Sonnet; near Opus 4.8 at $2/$10 (intro pricing made **permanent** Aug 10); default model on Free/Pro |
| **Claude Opus 5** | **2026‑07‑24** | — | — | — | 1M in / 128K out | C | Matches or exceeds original Fable 5 on several evals (vendor); GLM‑5.3 comparison table shows Opus 4.8‑era scores clearly surpassed | New **general‑purpose flagship**, replacing Opus 4.8: "close to Fable 5's frontier intelligence at half the price" ($5/$25). Five effort levels (low→max), fast mode at ~2.5× speed ($10/$50), knowledge cutoff May 2026. Default on Max, strongest model on Pro. Fixes the Fable 5 complaints: fewer refusals/fallbacks, cheaper, no 30‑day retention. Shipped with mid‑conversation tool changes + automatic safety fallbacks (beta) |

| **Claude Fable 5.1 / Mythos 5.1** | **2026‑09‑01** | — | — | — | 1M in / 128K out | C (Fable GA; Mythos trusted access) | Same weights. Anthropic: Terminal‑Bench 4.0 **55.8% Fable / 60.9% Mythos**, Terminal‑Bench‑Science 0.1 **52.6%**, SWE‑bench Pro **81.2%**, HLE **60.9% no tools / 65.0% with tools**, OSWorld 2.0 77.9% partial / 41.7% strict (Aug 2026 task set), AutomationBench 31.4%, CursorBench 3.2 73.4%, GDPval‑AA v2 **1853 Elo**, ARC‑AGI‑2 90.0%. System card also: SWE‑bench Multilingual 89.1% | Mythos‑class refresh. Cache reads cut to **$0.25/Mtok** (75% less; ~25% cheaper typical workloads, up to ~45% on highly agentic work); sticker price still $10/$50. Fable may discover vulnerabilities but exploit development reroutes to Opus. Mythos biology access is a **Life Sciences Verification Program** built with the US government; cyber access expands via the Cyber Verification Program. Mythos designed high‑affinity protein binders (~10× Adaptyv competition winners, ~50% hit rate) and a higher‑resolution elevation map of a third of Venus. Knowledge cutoff June 2026. Adaptive thinking always on |

Notes: From Aug 14 Anthropic began watermarking Claude text output to comply with the EU AI Act's transparency code (in force Aug 2, ~190 signatories including all major Western labs). Fable 5.1 and Mythos 5.1 share weights; score gaps on Terminal‑Bench 4.0 are mostly the cyber safeguards firing. OpenAI's launch table and Anthropic's system card agree on Fable 5.1 Terminal‑Bench 4.0 at 55.8%; xAI's Grok 4.7 table lists Fable 5.1 at 57.9% on the same benchmark name — treat cross‑lab harnesses as not directly comparable.

Sources: [Anthropic news](https://www.anthropic.com/news), [Opus 5](https://www.anthropic.com/research/claude-opus-5), [Text watermarking](https://www.anthropic.com/news/claude-text-watermark), [Opus 4.5](https://www.anthropic.com/news/claude-opus-4-5), [Sonnet 4.5](https://www.anthropic.com/news/claude-sonnet-4-5/), [Fable 5 / Mythos 5](https://www.anthropic.com/news/claude-fable-5-mythos-5), [Redeploying Fable 5](https://www.anthropic.com/news/redeploying-fable-5), [Sonnet 5](https://www.anthropic.com/news/claude-sonnet-5), [Opus 4.1 system card](https://www.anthropic.com/claude-opus-4-1-system-card), [Models overview docs](https://docs.anthropic.com/en/docs/about-claude/models/whats-new-claude-4-5), [Artificial Analysis: Opus 4.5](https://artificialanalysis.ai/articles/claude-opus-4-5-benchmarks-and-analysis), [W&B: Opus 4.8 benchmarks](https://wandb.ai/byyoung3/ml-news/reports/Claude-Opus-4-8-Benchmark-Scores--VmlldzoxNzA0NTk3MQ), [Epoch AI](https://epoch.ai/data-insights/models-over-1e25-flop).

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
| **Gemini 3.5 Pro** | limited preview; **still not GA as of 2026‑09‑23** | — | — | — | 1M | C | — | Announced at I/O; repeatedly delayed — reporting cites coding/reliability problems; Flash line carries the brand in the meantime |
| **Gemini 3.6 Flash + 3.5 Flash‑Lite + 3.5 Flash Cyber** | 2026‑07‑21 | — | — | — | 1M | C | Improved token efficiency; Cyber variant tuned for defensive security work | Start of an "almost monthly" Flash cadence (Pichai, Q2 earnings call); same post confirmed **Gemini 4 pre‑training has begun** ("our most ambitious pre‑training run yet" — larger base model, coding + agents priorities); $1.50/M input |
| **Gemini 3.7 Flash** | 2026‑08 (mid) | — | — | — | 1M | C | DeepSWE ≈65% | Second beat of the monthly Flash cadence; frontier‑adjacent agentic coding from the cheap tier |
| **Gemini 3.8 Flash** | **2026‑09‑02** | Based on 3.7 Flash (not a new base) | — | — | 1M in / 64K out | C | Model card: DeepSWE v1.1 **73.7%**, Terminal‑Bench 2.1 89.4%, Terminal‑Bench 4.0 **19.1%** (Opus 5 51.8%, Sol 37.3% in the same card), HLE‑Verified 54.9%, OSWorld‑2.0 59.0% partial, GDPval‑AA v2 1545 Elo, BioMysteryBench human‑difficult 56.5%. OpenAI's table: GPQA Diamond 95.3% | Third Flash in six weeks. Intro price $0.75/$3.75 per Mtok through Dec 31, 2026, then $1.50/$7.50. Knowledge cutoff March 2026. Google's Frontier Safety assessment: no meaningful new capability vs 3.7 Flash; unlikely to reach a Tracked or Critical level. Same day: **Gemini 3.8 Flash Cyber**, via the new **Fairwind Program** for trusted defenders — CyberGym "frontier," CWE‑Bench pass@1 47.2% vs Fable 5 at 47.8%. TTS variants (Flash and Flash‑Lite) followed Sep 23; not frontier text models |

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
| **Muse Spark 1.2 + Muse Code (beta)** | 2026‑08‑05 | undisclosed | — | — | 1M | C | AA Intelligence Index 54 (14th of 186); "moderate improvement" (Meta's own words) on multi‑file refactors and long debugging | Meta's **first coding agent**: Muse Code (terminal, macOS/Linux) was **co‑trained with the model** — compaction, goals, and subagent structure optimized against the harness, not bolted on. Replay‑exact event log; persistent session subagents. Global API access opened; new **contributor tier** at $0.10/$0.20 per Mtok where prompts may train Meta models — data‑for‑discount as explicit pricing |
| **Muse Glimmer 30B** | announced 2026‑08‑10 | 30B | — | — | — | **OW (Apache‑2.0)** | Agentic reliability on 24GB VRAM | Meta's first open weights of the Muse era; open‑weight Muse Spark 1.2 promised "soon" (no date, no license yet) |
| **Muse Spark 1.3** | **2026‑09‑02** | undisclosed | — | — | 1M | C | No public score table in the launch post ("see our report"). Internal engineering comparisons vs 1.2: ~20% fewer tool calls, ~25% fewer tokens, less verbose | Long‑horizon agent post‑train: better at multi‑workflow threads, clarifying questions, and not hallucinating past its limits. Available in Muse Code and the Meta Model API at max reasoning |

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
| **DeepSeek‑V4 Flash** | 2026‑04‑24 (preview) | 284B / 13B active MoE | — | — | 1M | OW (MIT) | SWE‑bench Verified ≈79% | Cost‑efficient sibling ($0.14/$0.28 per Mtok); many production stacks route cheap traffic here |
| **DeepSeek‑V4‑Flash‑0731** (official) | **2026‑07‑31** | ~300B / 13B active MoE | — | — | 1M (384K out) | OW (MIT; 166.9 GB, 48 shards) | Terminal‑Bench 82.7 (vendor, hosted); beats V4‑Pro‑Preview on several agent evals | Same architecture, re‑post‑trained for agents; native Responses API + first‑class **Codex integration** (first non‑OpenAI model with a dedicated Codex guide); still $0.14/$0.28 — "cheapest model to run in its class" |
| **DeepSeek‑V4‑Pro‑0813** (GA) | **2026‑08‑13** | 1.6T / 49B active MoE | — | — | 1M (384K out) | OW (MIT) | Terminal‑Bench 2.1 87.9, DeepSWE 62.7, NL2Repo 61.5 (vendor, unreplicated) | V4 generation complete. GA arrived as a quiet version‑string change; days later DeepSeek **raised API prices and introduced peak/off‑peak billing** (off‑peak = half price, from Aug 16) — the end of the subsidized‑inference era that made DeepSeek famous |
| **DeepSeek‑V4‑Flash‑Vision‑Exp** | 2026‑08‑21 | — | — | — | — | API (experimental) | — | First multimodal vision model in the V4 line. Retired Sep 10; the name now routes to V4.1‑Flash |
| **DeepSeek‑V4.1‑Flash** | **2026‑09‑10** | **552B backbone / 8B active on prefill, 16B on decode**; plus a 196B Engram memory | Pretrained on **45T** multimodal tokens | — | **1M** | **OW** (Hugging Face) | API changelog, max effort: GPQA Diamond 90.9, HLE 36.8 (39.1 text‑only), **HLE with tools 63.9**, Codeforces 3471, Terminal‑Bench 2.1 **90.6**, Terminal‑Bench 3.0 **30.0**, Terminal‑Bench 4.0 31.2, DeepSWE v1.1 **74.2**, CyberGym 88.1, AutomationBench 54.8, Agents' Last Exam 31.8 | New **Causal Encoder–Decoder**: decode activates twice the parameters of prefill, aimed at input‑heavy agents. Global KV cache ~890 bytes/token, about a quarter of V4‑Flash. DeepSeek says it beats V4‑Pro on cost, speed, and quality, and from **Sep 14** routes `deepseek-v4-pro` to Flash at Flash prices until V4.1‑Pro. Prices cut the same day; off‑peak remains half of peak. API id `deepseek-flash` |

Note: DeepSeek never shipped a model branded "R2" (still true as of September 2026 — Reuters reported Liang Wenfeng held it back over performance; some third‑party "R2 launch" posts in May 2026 are unreliable). V3.1 unified reasoning + non‑reasoning into one model. The hosted R1 endpoint retired July 24, 2026. As of Sep 14, 2026 the V4‑Pro API itself is a compatibility alias for V4.1‑Flash.

Sources: [DeepSeek API change log](https://api-docs.deepseek.com/updates/), [BentoML DeepSeek guide (2026)](https://www.bentoml.com/blog/the-complete-guide-to-deepseek-models-from-v3-to-r1-and-beyond), [DeepSeek‑V3.2 paper (arXiv 2512.02556)](https://arxiv.org/html/2512.02556v1), [V3.2 release notes](https://api-docs.deepseek.com/news/news251201), [Reuters on R1 cost](https://www.reuters.com/world/china/chinas-deepseek-says-its-hit-ai-model-cost-just-294000-train-2025-09-18/), [The Register on full cost](https://www.theregister.com/2025/09/19/deepseek_cost_train/).

---

## xAI / SpaceXAI

Corporate note: SpaceX absorbed xAI in a February 2026 all‑stock deal (~$1.25T combined) and rebranded the unit **SpaceXAI** in May 2026. SpaceX IPO'd on Nasdaq June 12 ($75B raised, largest ever). The ~$60B all‑stock Anysphere (Cursor) acquisition **closed August 14, 2026**. Grok 5 (reportedly ~6T) was still described as in training on Colossus 2 as of late August; Grok 4.7 (Sep 21) is a new, larger base than 4.6, but xAI has not said it is Grok 5.

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
| **Grok 4.6** | **2026‑08‑12** | ~1.5T (same base as 4.5; post‑training upgrade) | — | — | **500K** | C | **GPQA Diamond 94.9% (record at the time; GPT‑6 Astra later posted 96.0%)**, AA Intelligence Index 61 (tied GPT‑5.6 Sol max, tied 3rd overall), GDPval‑AA v2 + AA‑Briefcase 1577 Elo (2nd); trails on DeepSWE and Terminal‑Bench | Post‑train focused on **long‑running agents**: regenerated SFT trajectories, RL in agentic environments, trained on agent‑failure data; checks its own work mid‑task; new `xhigh` effort. Same $2/$6 (fast variant 2×; rates double past 200K prompt tokens). First flagship built ground‑up under the SpaceXAI name, co‑developed with Cursor |
| **Grok 4.7** | **2026‑09‑21** | New, larger base than 4.6 (count undisclosed) | Longer RL on multi‑hour tasks | — | **500K** | C | xAI table, xHigh unless noted: CursorBench 4.0 **46.3%** (Fable 5.1 51.8%, Sol 41.7%, Grok 4.6 40.4%), DeepSWE v1.1 71.0% (high, not xHigh), Terminal‑Bench 4.0 **37.6%** (Grok 4.6 20.3%), EEBench **64.0%**, AA Briefcase v1.1 1657, Harvey Legal Agent 19.6%, HealthBench Professional 56.7%. LatchBio biosafety **62.4%** | Same $2/$6 as 4.6; fast variant 2× speed at 2× price. New safeguard stack. HackerBench v0.3: 3.3% of risky dual‑use cyber prompts pass. Invite‑only red‑team cyber access for selected partners. Available in Cursor, Grok Build, and the API |

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
| **Qwen3.8‑Max** | **2026‑08‑03** (previewed at WAIC Jul 19) | **2.4T / 95B active** MoE (512 experts, hybrid GatedDeltaNet + gated attention) | — | — | 1M (hosted) | C (hosted) → weights Aug 12 | PaperBench 93%, OSWorld‑Verified 86.1%, BabyVision 82, Terminal‑Bench 2.1 86.6; 5th Text Arena, 2nd Vision Arena at launch | Largest model Alibaba has built; hybrid thinking; vision + video input; $2/$6 per Mtok |
| **Qwen3.8‑2.4T‑A95B** (open checkpoint) | **2026‑08‑12** | 2.4T / 95B active | — | — | 262K (extensible 1M) | **OW (custom `qwen3.8‑max` license)** | Text‑only, thinking‑mode‑only version of the above | **First Qwen‑Max‑class flagship ever open‑weighted** — among the largest weights ever published (with Kimi K3); hosted Max keeps vision, non‑thinking mode, and native 1M for itself. Apache‑2.0 Qwen3.8‑27B followed Aug 14 |

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
| **Shieldstral 1.0 (3B)** | 2026‑08‑04 | 3.8B | — | — | 32K | OW (Apache‑2.0) | Text safety F1 84.9% (matches GPT‑OSS‑Safeguard‑20B); multimodal moderation SOTA | Policy‑adaptive safety classifier — moderation policy written in plain language at inference time; single 16GB GPU; inaugural release of the NVIDIA‑led Open Secure AI Alliance. Also in the window: Leanstral 1.5 (machine‑checked proofs, Jul) and OCR 4.1 (Aug 13) |

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
| **Kimi K3** | **2026‑07‑16** (hosted API) → weights **2026‑07‑27** | **2.8T total / 104B active** MoE (multimodal, quantization‑aware trained) | — | — | **1M** | **OW (custom "Kimi K3 License"** — free below $20M/yr MaaS revenue; attribution above 100M MAU; AA labels it "Commercial Use Restricted") | **AA Intelligence Index 57 — #4 of 189 overall, top open model at release**; behind only Fable 5 and two GPT‑5.6 Sol settings, ahead of Opus 4.8 and GPT‑5.5; leads Arena Code WebDev; Terminal‑Bench 2.1 88.3, DeepSWE 67.5, Toolathlon 76.5 | **Largest open‑weights model ever released** (1.56 TB, 96 shards); world's first open 3T‑class model per Moonshot; $3/$15 API. Geopolitical flashpoint: White House science adviser Kratsios claimed (Jul 22) K3 was **distilled from Claude Fable 5**; Treasury Secretary Bessent threatened sanctions; researchers noted the timeline made distillation implausible |

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
| **GLM‑5.2** | 2026‑06‑13 | Zhipu / Z.ai | 744B/40B MoE | 1M | OW (MIT) | SWE‑bench Pro 62.1% — strongest open coding model on that board at release |
| **GLM‑5.3** | **2026‑08‑14** | Zhipu / Z.ai | same 744B/40B base as 5.2 — **all gains from post‑training** | 1M | API at launch; open weights were promised ~2 weeks later and were **not confirmed public as of Sep 23** | AA Index 60 at launch; **GDPval‑AA v2 1769 Elo** — led Fable 5 (1743) and GPT‑5.6 Sol (1730) in August; **Fable 5.1 took the lead in September at 1853**. Terminal‑Bench 2.1 88.2; Terminal‑Bench 3.0 28.3 (open SOTA until DeepSeek V4.1‑Flash posted 30.0); DeepSWE 66.9; HLE w/ tools 62.5 |
| **MiniMax‑H3** | 2026‑07 (late) | MiniMax | undisclosed MoE | 200K+ | OW | Multimodal successor to M3 |
| **Phi‑5 Mini / Medium 14B** | 2026‑05 / 2026‑05‑30 | Microsoft | 4B / 14B | 64K→256K | OW (MIT) | Medium: MMLU 86%, AIME 2025 75% — GPT‑4‑class at 14B |
| **Stripe of Chinese OW frontier**: Yi, GLM, Doubao, Qwen, DeepSeek, Kimi, MiniMax | 2024–2026 | various | various | — | mostly OW | Closed the gap with US frontier in 2025–2026 |

---

## Key takeaways

1. **Compute scaling continued**: From GPT‑3 (~3e23 FLOP) to GPT‑4 (2.1e25) to GPT‑4.5 (6.4e25) and clearly past 1e26 for GPT‑5/Gemini 3 (numbers undisclosed but inferable from cluster size and training duration). Epoch AI tracked >30 models above 1e25 FLOP by mid‑2025.
2. **Costs flattened from the developer's perspective**: DeepSeek V3 was trained for ~$5.6M (Dec 2024) and matched many Western frontier models. Anthropic confirmed Claude 3.5 Sonnet and 3.7 Sonnet each cost "tens of millions" — far below the rumored hundreds of millions for GPT‑4.5. Frontier *capabilities* are getting cheaper to reproduce even as raw frontier *compute* keeps climbing.
3. **The reasoning paradigm shift** (Sep 2024 → present): o1‑preview kicked off explicit "thinking" models. By 2026 every frontier vendor ships hybrid (instant + thinking + pro) models with parallel test‑time compute — and mid‑2026 pushed it further into **multi‑agent test‑time compute** (GPT‑5.6 `ultra` coordinating 4–16 parallel agents, Claude Dynamic Workflows with hundreds of subagents, Kimi K2.6 300‑agent swarms).
4. **Benchmark saturation**: MMLU and HumanEval are saturated. In September 2026, ARC‑AGI‑3 (7.8% → 99.9%), FrontierMath Tier 4 (→ 97.6%), and ARC‑AGI‑2 (→ 95%) joined them, all on OpenAI's GPT‑6 Astra launch table. What still discriminates: Terminal‑Bench 4.0 (Mythos 5.1 60.9%, Astra 57.9%, Gemini 3.8 Flash 19.1%), Terminal‑Bench 3.0 (still ~35%), Humanity's Last Exam with tools (Fable 5.1 65.0%; Astra 57.2% on OpenAI's own table), SWE‑bench Pro, and long‑horizon professional work (GDPval‑AA). Artificial Analysis Intelligence Index **v4.1.1** is a new version — do not compare its 61–66 cluster to the older index numbers cited for July–August models.
5. **Open weights closed most of the gap** in 2025–2026 — and in July–August 2026 the gap functionally closed at the trillion‑parameter scale. In four weeks Chinese labs shipped **Kimi K3 (2.8T, weights Jul 27), Qwen3.8‑Max (2.4T, weights Aug 12), DeepSeek V4‑Pro GA (1.6T, Aug 13), and GLM‑5.3 (Aug 14)**. Open models now score 57–60 on the AA Intelligence Index against 61–65 for the best closed settings, and GLM‑5.3 *tops* GDPval‑AA v2 outright. Every open flagship now ships under a custom commercial‑threshold license rather than Apache/MIT (Kimi K3 License, `qwen3.8‑max`) — "open" increasingly means "downloadable." Meanwhile Meta's frontier line (Muse Spark, closed, paid API) sits *above* its open Llama line.
6. **Context windows exploded**: from 4K (2022) → 128K (2023) → 1M (Gemini 1.5, 2024) → 10M (Llama 4 Scout, 2025) → native 1M as table stakes even for open models (DeepSeek V4, Qwen 4, Gemma 4.5, Claude 4.6+, Gemini 3.x).
7. **Government entered the release loop** (2026): Anthropic's Fable 5 / Mythos 5 were suspended for 18 days under a US export‑control directive (June 12–30). GPT‑5.6 launched via a government‑coordinated preview. On Sep 3–4 GPT‑6 Astra shipped **after** OpenAI confirmed the Critical cyber threshold, with the public model refusing some cyber prompts. Fable 5.1 (Sep 1) may discover vulnerabilities but not develop exploits; Mythos 5.1 biology access is a US‑government life‑sciences program. Google opened Fairwind the next day for Gemini 3.8 Flash Cyber. The pattern is now: ship the model, and ship a vetted‑access lane beside it.
8. **The pre‑training pause ended in September.** No Western lab shipped a new frontier base between GPT‑5.6 / Fable 5 (June) and late August — Opus 5, Grok 4.6, and Muse Spark 1.2 were post‑trains. Then, inside three weeks: GPT‑6 Astra (new pretrain, >100k GPUs at Stargate), Grok 4.7 (new larger base), and DeepSeek V4.1‑Flash (new Causal Encoder–Decoder, which then replaced the 1.6T V4‑Pro API). Gemini 3.8 Flash and Muse Spark 1.3 were still post‑trains. Gemini 4 and Grok 5 remain unreleased.
9. **AI started producing new mathematics, then saturated the math benchmarks.** OpenAI's Aug 1 Astra note claimed ten new machine‑checked results. On Sep 3 the shipped model scored 97.6% on FrontierMath Tier 4 (v2) and 99.9% on ARC‑AGI‑3. Capability and deployment are no longer the same event: the math landed in August; the product, and the cyber gate, landed in September.

---

## Primary sources

- [Epoch AI — Notable AI Models database](https://epoch.ai/data/ai-models)
- [Epoch AI — >1e25 FLOP tracker (June 2025)](https://epoch.ai/data-insights/models-over-1e25-flop)
- [Epoch AI — Tracking large‑scale AI models](https://epoch.ai/blog/tracking-compute-intensive-ai-models)
- OpenAI: [Release notes](https://help.openai.com/en/articles/6825453-chatgpt-release-notes), [GPT‑5](https://openai.com/index/introducing-gpt-5/), [GPT‑5.2](https://openai.com/index/introducing-gpt-5-2/), [GPT‑6 Astra](https://openai.com/index/gpt-6-astra/)
- Anthropic: [News index](https://www.anthropic.com/news), [Fable 5.1 and Mythos 5.1](https://www.anthropic.com/claude-fable-and-mythos-5-1), [Models docs](https://docs.anthropic.com/en/docs/about-claude/models/whats-new-claude-4-5)
- Google DeepMind: [Gemini 3](https://deepmind.google/blog/a-new-era-of-intelligence-with-gemini-3/), [model cards](https://deepmind.google/models/), [Gemini API changelog](https://ai.google.dev/gemini-api/docs/changelog)
- Meta: [Llama 4 launch](https://ai.meta.com/blog/llama-4-multimodal-intelligence)
- DeepSeek: [API change log](https://api-docs.deepseek.com/updates/), [V4.1‑Flash](https://api-docs.deepseek.com/news/news260910), [V3.2 paper (arXiv 2512.02556)](https://arxiv.org/html/2512.02556v1)
- xAI: [Grok 4](https://x.ai/news/grok-4), [Grok 4.7](https://x.ai/news/grok-4-7)
- Alibaba: [Qwen3‑Max‑Thinking blog](http://www.alibabacloud.com/blog/pushing-qwen3-max-thinking-beyond-its-limits_602834)
- Mistral: [Large 2](https://mistral.ai/fr/news/mistral-large-2407), [Medium 3](https://mistral.ai/news/mistral-medium-3)
- Moonshot AI: [Kimi K2 Thinking blog](https://kimi-k2.org/blog/15-kimi-k2-thinking-en)
- Independent benchmark services: [Artificial Analysis](https://artificialanalysis.ai/), [LMArena](https://lmarena.ai/), [ARC Prize](https://arcprize.org/), [Vellum benchmarks](https://www.vellum.ai/blog/), [APXML](https://apxml.com/), [DocsBot](https://docsbot.ai/)

_Compiled April 26, 2026; updated July 9, 2026; updated August 23, 2026; updated September 23, 2026 (GPT‑6 Astra, Claude Fable 5.1 / Mythos 5.1, Gemini 3.8 Flash + Flash Cyber, Muse Spark 1.3, DeepSeek V4.1‑Flash, Grok 4.7). Treat all undisclosed compute, parameter, and cost figures as approximate; mark them as such when citing._
