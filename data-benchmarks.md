# AI Benchmark Saturation Timeline (2020 → August 2026)

A research compilation of how 14 major AI benchmarks have evolved from "released as hard" to (in many cases) saturated. Compiled April 26, 2026; updated July 9, August 23, and September 23, 2026.

> **Caveats up front.** Numbers come from a mix of vendor-reported model cards, third-party leaderboard aggregators (Vals AI, Artificial Analysis, lmarena.ai, Epoch AI, BenchLM, llm-stats, papers-with-code) and the original benchmark papers. Where vendor numbers and independent evaluations diverge, both are noted. Late-2025/early-2026 numbers from aggregators like BenchLM, TokenMix, lmmarketcap, intuitionlabs etc. should be treated as best-effort secondary reporting; some include forward-looking models (e.g. "Claude Mythos Preview", "GPT-5.4", "Gemini 3.1 Pro") whose system cards are still being independently re-benchmarked. Top-of-leaderboard differences of 1-2 points are routinely within inter-run variance.

---

## TL;DR — Saturation status as of September 2026

| Benchmark | Released | Top score 2026 | Status | Time-to-saturation |
| --- | --- | --- | --- | --- |
| MMLU | Sep 2020 | ~92% (GPT-5.4, Claude Opus 4.6) | **Saturated** (>90% cluster, <89.8% human expert breached) | ~4 yr (2020 → 2024) |
| HumanEval | Jul 2021 | ~95-98% (with scaffolding) | **Saturated** (no longer differentiates) | ~3 yr (2021 → 2024) |
| GSM8K | Oct 2021 | ~97-99% (multiple models) | **Saturated** | ~3 yr (2021 → 2024) |
| MATH (Hendrycks) | Oct 2021 | ~97-99% (GPT-5.2 Pro, o3) | **Saturated** | ~3-4 yr (2021 → 2024-25) |
| BIG-Bench Hard (BBH) | Oct 2022 | ~94% (Claude Sonnet 4.5) | **Saturated** (BBEH is successor) | ~3 yr (2022 → 2025) |
| GPQA Diamond | Nov 2023 | 96.0% (GPT-6 Astra, Sep 3) | **Saturated** (>>69.7% PhD experts) | ~2.5 yr (2023 → 2026) |
| SWE-bench Verified | Aug 2024 | ~88-94% (Opus 4.8, Claude Mythos) | **Mostly solved** (Pro variant is current frontier) | ~1.5 yr (2024 → 2026) |
| SWE-bench Pro | Late 2025 | 81.2% vendor-scaffold (Fable 5.1) / ~59% standardized (Scale, earlier) | **Partially solved** — current frontier coding benchmark | Open |
| Terminal-Bench 2.x | 2025 | 91.9% (GPT-5.6 Sol ultra); 2.1 top cluster 87-89% across 6 labs | **Saturating** — six models within ~1pp by Aug 2026 | ~1 yr |
| Terminal-Bench 3.0 | 2026 (Jul) | 34.6% (GPT-5.6 Sol); open 30.0% (DeepSeek V4.1-Flash, was 28.3% GLM-5.3) | **Hard** | Open |
| Terminal-Bench 4.0 | 2026 (Sep) | 66.4% (Claude Opus 5.5, xhigh); 57.9% (GPT-6 Astra, high); 19.1% (Gemini 3.8 Flash) | **Hard** — effort levels are not aligned across labs | Open |
| ARC-AGI-1 | 2019/2024 (semi-private set) | 87.5% (o3 high-compute, late 2024) | **Saturated** | ~5 yr (2019 → 2024) |
| ARC-AGI-2 | Mar 2025 | 95.0% (GPT-6 Astra) | **Saturated** (human baseline ~60% was crossed in Feb 2026) | ~1.5 yr |
| ARC-AGI-3 | 2026 | 99.9% (GPT-6 Astra; 7.78% for GPT-5.6 Sol a month earlier) | **Fell in one release** — ARC Prize: human action-efficiency baseline beaten on 96% of levels | ~months |
| AIME 2024/2025 | Annual | 99-100% (GPT-5.2 Pro, w/tools) | **Saturated** | ~1-2 yr |
| FrontierMath (Tier 1-3) | Nov 2024 | ~89% (GPT-5.6 Sol, v2) | **Mostly solved** (was <2% on release) | ~1.5 yr |
| FrontierMath (Tier 4) | Jul 2025 | 97.6% (GPT-6 Astra, v2, Sep 3) | **Saturated** on the v2 set (was ~19% in April, ~83-88% in July) | ~1 yr |
| Humanity's Last Exam | Jan 2025 | 67.7% with tools (Claude Opus 5.5); Fable 5.1 65.6% in the same Sep 22 table; Astra 57.2% on OpenAI's table; open 63.9% (DeepSeek V4.1-Flash) | **Partially solved** (was 2.7% on release) | Open |
| MMMU (original) | Jan 2024 | ~79% | **Saturated**, MMMU-Pro is successor | ~2 yr |
| MMMU-Pro | Sep 2024 | ~88-94% (Gemini 3.1 Pro Preview, GPT-5.4 Pro) | **Approaching saturation** (88.6% best human expert) | ~1.5 yr |
| LiveCodeBench | Mar 2024 | ~85-89% (Gemini 3.1 Pro Preview, GPT-5.x Codex) | **Approaching saturation** (Pro variant still discriminates) | ~2 yr |
| Chatbot Arena Elo | May 2023 | ~1500-1537 (Claude Opus 4.6/4.7, Gemini 3.1 Pro) | **No ceiling** (relative ranking, not %) | N/A |

**Pattern: most "hard" benchmarks released between 2020-2023 saturated within 2-4 years.** Benchmarks released in 2024-2025 (HLE, FrontierMath, ARC-AGI-2, SWE-bench Pro) are already partially solved.

---

## 1. MMLU (Massive Multitask Language Understanding)

- Released: September 2020 by Hendrycks et al. (ICLR 2021).
- 57 academic subjects, undergraduate-to-graduate.
- Human expert estimate: **89.8%**.

| Date | Model | Score | Notes |
| --- | --- | --- | --- |
| 2020 (Sep) | GPT-3 175B (few-shot) | 43.9% | Original paper |
| 2020 | GPT-3 175B (fine-tuned) | 53.9% | Original paper |
| 2021 (Dec) | Gopher 280B | 60.0% | DeepMind |
| 2022 | Chinchilla 70B | 67.5% | DeepMind |
| 2022 (Apr) | PaLM 540B | 69.3% | Google |
| 2022 (Nov) | GPT-3.5 | ~70% | OpenAI |
| 2023 (Mar) | GPT-4 | 86.4% | Crossed below human; OpenAI report |
| 2023 (Dec) | Gemini Ultra | 90.0% | Google (CoT@32, contested) |
| 2024 (Jun) | Claude 3.5 Sonnet | ~88.7% | Anthropic |
| 2024 (Sep) | o1-preview | 92.3% | First reasoning model; AI Index 2025 |
| 2024-2026 | Frontier cluster (GPT-4o, GPT-5, Gemini 2.5 Pro, Claude Opus 4.x, DeepSeek V3+) | 88-92% | Saturated; <2-3 pt differentiation |
| 2026 (Apr) | GPT-5.4 / Claude Opus 4.6 | ~91.8-92.1% | Within statistical tie |

**Sources:** [Hendrycks 2020 paper](https://arxiv.org/abs/2009.03300) · [MMLU Wikipedia](https://en.wikipedia.org/wiki/MMLU) · [Stanford AI Index 2025 ch.2](https://hai.stanford.edu/assets/files/hai_ai-index-report-2025_chapter2_final.pdf) · [TokenMix 2026 leaderboard](https://tokenmix.ai/blog/mmlu-benchmark-leaderboard) · [BenchLM MMLU 2026](https://benchlm.ai/benchmarks/mmlu)

> **Successor: MMLU-Pro** (10 choices, harder questions). Top scores ~78% (GPT-5.4) to ~89.8% (Gemini 3 Pro Preview, April 2026). Frontier cluster spread: 14-16 points lower than MMLU.

---

## 2. HumanEval

- Released: July 2021 by Chen et al. (OpenAI Codex paper).
- 164 hand-written Python problems; pass@1 metric.

| Date | Model | pass@1 | Notes |
| --- | --- | --- | --- |
| 2021 (Jul) | GPT-3 | 0% | Pre-Codex baseline |
| 2021 (Jul) | Codex 12B | 28.8% | Original paper |
| 2022-2023 | Various (PaLM, Codex variants) | 50-60% | Mid-range progression |
| 2023 (Mar) | GPT-4 | 67% | OpenAI technical report |
| 2024 (Mar) | Claude 3 Opus | 84.9% | Anthropic |
| 2024 (May) | GPT-4o | ~90% | OpenAI |
| 2024 (Jun) | Claude 3.5 Sonnet | 92.0% | Anthropic |
| 2024 (Sep) | o1-preview / o1-mini | 96.3% | OpenAI; effectively saturated |
| 2024-2025 | Scaffolded variants (LDB+GPT-4o, AgentCoder) | 96-98% | pass@1 with agentic loops |
| 2026 | GPT-5.4 / Claude Opus 4.6 / GPT-5.3 Codex | 91-95% | Vendor-reported; benchmark deprecated |

**Sources:** [Chen et al. 2021 paper](https://arxiv.org/abs/2107.03374) · [Klu HumanEval](https://klu.ai/glossary/humaneval-benchmark) · [Runloop "When Machines Learned to Code"](https://www.runloop.ai/blog/humaneval-when-machines-learned-to-code) · [BenchLM coding 2026](https://benchlm.ai/coding)

> **Status**: Saturated. Now a "baseline competency test". Replaced by SWE-bench Verified, LiveCodeBench, and BigCodeBench for frontier model differentiation.

---

## 3. GSM8K (Grade School Math 8K)

- Released: October 2021 by Cobbe et al. (OpenAI).
- 8.5K grade-school word problems requiring 2-8 step arithmetic reasoning.

| Date | Model | Score | Notes |
| --- | --- | --- | --- |
| 2021 (Oct) | GPT-3 175B | ~20% | CoT prompting |
| 2022 (Jun) | Minerva 540B | 78.5% | 8-shot, majority voting; Google |
| 2022 (Nov) | GPT-3.5 | 57% | 5-shot |
| 2023 (Mar) | GPT-4 | 92% | 5-shot CoT |
| 2023 (Dec) | Gemini Ultra | 94.4% | Maj. vote, 32 generations |
| 2024 (Mar) | Claude 3 Opus | ~95% | Zero-shot |
| 2024 (Jun) | Claude 3.5 Sonnet | 96.4% | Anthropic |
| 2024 (Jul) | Llama 3.1 405B | ~97% | Meta |
| 2025-2026 | Frontier cluster (Kimi K2, GPT-5, Claude Opus 4.x, o3-pro) | 97-99% | Saturated; mostly omitted from new model cards |

**Sources:** [Cobbe et al. 2021 paper](https://arxiv.org/abs/2110.14168) · [Klu GSM8K](https://klu.ai/glossary/GSM8K-eval) · [llmdb GSM8K](https://llmdb.com/benchmarks/gsm8k) · [LM Market Cap GSM8K](https://lmmarketcap.com/benchmarks/gsm8k)

> **Status**: Saturated by 2024. No longer reported on most new flagship model cards.

---

## 4. MATH (Hendrycks)

- Released: October 2021 by Hendrycks et al.
- 12,500 competition mathematics problems (AMC, AIME-level).

| Date | Model | Score | Notes |
| --- | --- | --- | --- |
| 2021 | GPT-3 | ~7% | Original paper baseline |
| 2022 (Jun) | Minerva 540B | 50.3% | Google |
| 2023 (Mar) | GPT-4 | 50.4% | OpenAI report |
| 2023 (Dec) | Gemini Ultra | 53.2% | Google |
| 2024 (May) | GPT-4o | 76.6% | OpenAI |
| 2024 (Sep) | o1 | 94.8% | First reasoning leap; +34.5 vs GPT-4o |
| 2024 (Dec) | o3 (preview) | ~96-97% | OpenAI |
| 2025 (Feb) | Claude 3.7 Sonnet | ~97% | Anthropic |
| 2025-2026 | GPT-5.2 Pro / o3-pro / Kimi K2 / Gemini 3 Pro | 97-99% | MATH-500 mostly solved; Vals AI stopped tracking |
| 2026 (Apr) | GPT-5.2 Pro | 99.0% | pricepertoken/Artificial Analysis |

**Human reference**: AIME-qualifying contestants ~75-90%; the AI Index 2025 noted SOTA was 7.9 pp above the original human comparison by 2024.

**Sources:** [Hendrycks 2021 paper](https://arxiv.org/abs/2103.03874) · [llmdb MATH](https://llmdb.com/benchmarks/math) · [Vals AI MATH-500](https://www.vals.ai/benchmarks/math500-04-11-2025) · [Stanford AI Index 2025](https://hai.stanford.edu/assets/files/hai_ai-index-report-2025_chapter2_final.pdf)

> **Status**: Saturated; data contamination concerns are now a top issue (problems are public).

---

## 5. BIG-Bench Hard (BBH)

- Released: October 2022 (Suzgun et al., Google) — 23-task subset of BIG-Bench where pre-2022 LMs underperformed humans.

| Date | Model | Score | Notes |
| --- | --- | --- | --- |
| 2022 | GPT-3.5 Turbo | 48.8% | Pre-CoT scaffolds |
| 2023 | GPT-4 Turbo | 66.8% | OpenAI |
| 2024 (Feb) | Gemini 1.5 Pro | 78.7% | Google |
| 2024 (Jul) | Llama 3.1 405B | 77.2% | Meta |
| 2024 (Dec) | DeepSeek V3 | 83.3% | DeepSeek |
| 2025-2026 | Claude Sonnet 4.5 / Gemini 3 Pro Preview / GLM-5 | 93-94% | Saturating |
| 2026 (Apr) | Claude Sonnet 4.5 | 94.4% | pricepertoken |

**Sources:** [BBH paper](https://arxiv.org/abs/2210.09261) · [BBEH paper (BBH successor)](https://arxiv.org/pdf/2502.19187) · [BenchGecko BBH](https://benchgecko.ai/benchmark/bbh) · [pricepertoken BBH 2026](https://pricepertoken.com/leaderboards/benchmark/bbh)

> **Successor: BIG-Bench Extra Hard (BBEH)** — Feb 2025. Best general model 9.8% harmonic, best reasoning model 44.8%. Confirmed BBH is now saturated.

---

## 6. GPQA Diamond

- Released: November 2023 by Rein et al. ("Graduate-Level Google-Proof Q&A").
- 198 questions, hardest "Diamond" subset of GPQA.
- **PhD expert baseline: 65% (paper) / 69.7% (OpenAI re-benchmark)**.

| Date | Model | Score | Notes |
| --- | --- | --- | --- |
| 2023 (Nov) | GPT-4 (zero-shot CoT) | ~39% | Original paper; below non-expert search baseline |
| 2024 (Mar) | Claude 3 Opus | ~60% | Crossed non-expert baseline |
| 2024 (Jun) | Claude 3.5 Sonnet | ~38.7% (single-sample) / 59.5% (32-vote) | Anthropic |
| 2024 (Sep) | o1 (zero-shot) | 77.3% | **First model to clearly beat PhD baseline** |
| 2024 (Sep) | o1-preview | ~33-34% (Sep eval) → updates later | Early variant |
| 2025 (Jan) | Claude Sonnet 4 | 78.2% | Anthropic |
| 2025 (Jul) | Grok 4 | ~87% (±2%) | Epoch AI evaluation |
| 2025 | Gemini 2.5 Pro | 86.4% | Google |
| 2025 (Q3) | GPT-5 | 88.4% | OpenAI |
| 2026 (Feb 5) | Claude Opus 4.6 | 91.3% | Anthropic |
| 2026 (Feb 19) | Gemini 3.1 Pro | 94.3% | Google DeepMind model card |
| 2026 (Apr 16) | Claude Opus 4.7 | 94.2% | Anthropic launch |
| 2026 (Apr) | Claude Mythos Preview | 94.6% | Secondary reporting (llm-stats) — not in primary paper |
| 2026 (Jul 9) | GPT-5.6 Sol | 94.6% | OpenAI launch table (Terra 92.9%, Luna 92.3%) — ties Mythos Preview |
| 2026 (Aug 12) | **Grok 4.6** | **94.9%** | Top score at the time; top-5 within 0.7pp |
| 2026 (Sep 3) | **GPT-6 Astra** | **96.0%** | OpenAI launch table. Same table: Gemini 3.8 Flash 95.3%, Sol 94.6%, Fable 5.1 93.7%, Opus 5 93.7%, Fable 5 92.6% |

**Sources:** [Rein et al. 2023 paper](https://arxiv.org/abs/2311.12022) · [IntuitionLabs GPQA Diamond](https://www.intuitionlabs.ai/articles/gpqa-diamond-ai-benchmark) · [SmartChunks GPQA explained](https://smartchunks.com/gpqa-diamond-score-explained-ai-benchmark-2026/) · [BenchGecko GPQA](https://benchgecko.ai/benchmark/gpqa-diamond)

> **Status**: Saturated. The top of the board moved from a 0.5 pp cluster around 94.5% to 96.0% (Astra). Still well above the 69.7% PhD-expert baseline, and no longer a place models separate by more than a couple of points.

---

## 7. SWE-bench / SWE-bench Verified

- SWE-bench released October 2023 (Princeton, Jimenez et al.) — 2,294 real GitHub Python issues.
- SWE-bench Verified released August 2024 by OpenAI — 500 human-validated subset.
- SWE-bench Pro released ~late 2025 — 1,865 multi-language tasks, contamination-resistant.

| Date | Model / System | SWE-bench Verified | Notes |
| --- | --- | --- | --- |
| 2023 (Oct) | GPT-4 (BM25 retrieval) | 1.96% (full SWE-bench) | Original paper |
| 2023 (Oct) | Claude 2 (oracle) | 4.8% | Original paper |
| 2024 (Mar) | Devin (Cognition) | 13.86% (full) / ~4.8% under indep. eval | Marked "AI software engineer" milestone |
| 2024 (May) | Claude 3 Opus | 22% | Anthropic |
| 2024 (Jun) | Claude 3.5 Sonnet (old) | 33% | Anthropic |
| 2024 (Aug) | Prior SOTA (Verified release) | 45% | OpenAI baseline |
| 2024 (Oct) | Claude 3.5 Sonnet (new) | **49%** | Anthropic; first widely-cited number |
| 2024 (Dec) | o1 / o1-preview | ~49% | OpenAI |
| 2025 (Mar) | Claude 3.5 Sonnet v2 | 55.2% | Anthropic |
| 2025 (Aug) | GPT-5 | 74.9% | OpenAI |
| 2025 (Q4) | Claude Opus 4.1 | 74.5% | Anthropic |
| 2025 (Nov) | Claude Opus 4.5 | 80.9% | Anthropic |
| 2025 (Dec) | GPT-5.2 | 80.0% | OpenAI |
| 2026 (Feb) | Claude Opus 4.6 / Gemini 3.1 Pro | 80.6-80.8% | Cluster within ~1 pp |
| 2026 (Apr) | Claude Mythos Preview | 93.9% | BenchLM/Anthropic |
| 2026 (Apr) | Claude Opus 4.7 (Adaptive) | 87.6% | Anthropic |
| 2026 (Apr) | GPT-5.3 Codex | 85% | OpenAI |
| 2026 (May 28) | Claude Opus 4.8 | 88.6% | Anthropic (95.0% per Vals AI independent) |

**SWE-bench Pro (Jul 2026):** vendor-scaffold aggregate (llm-stats — self-reported, comparable to each other, not to Scale's standardized board): Claude Fable 5 **80.0-80.3%** · Mythos Preview 77.8% · Opus 4.8 69.2% · GPT-5.6 Sol 64.6% · Grok 4.5 64.7% · Sonnet 5 63.2% · GLM-5.2 (OW) 62.1% · Qwen 3.7 Max 60.6% · GPT-5.5 58.6% · Kimi K2.6 (OW) 58.6%. Scale's standardized public-set leader: GPT-5.4 (xhigh) 59.1%. The frontier benchmark for agentic coding lives here; vendor scaffolding inflates ~10-20pp over the neutral harness.

**Sources:** [SWE-bench paper 2023](https://arxiv.org/abs/2310.06770) · [Anthropic Claude 3.5 Sonnet on SWE-bench](https://www.anthropic.com/research/swe-bench-sonnet) · [DEV: SWE-bench scores 2026](https://dev.to/rahulxsingh/swe-bench-scores-and-leaderboard-explained-2026-54of) · [BenchLM SWE-bench](https://benchlm.ai/benchmarks/sweVerified) · [theaiforger.com SWE-bench Verified](https://theaiforger.com/benchmarks/swe-bench-verified) · [Epoch AI 2025 forecasting recap](https://epoch.ai/gradient-updates/how-well-did-forecasters-predict-2025-ai-progress)

> **Status**: Verified is mostly solved (frontier ~80% with vendor-reported numbers up to 94%). Pro is the new frontier coding benchmark; expected to last 1-2 years.

---

## 8. ARC-AGI (Abstraction and Reasoning Corpus)

- ARC-AGI-1: François Chollet, 2019 ("On the Measure of Intelligence"). Public/private/semi-private splits.
- ARC-AGI-2: Launched March 2025 alongside ARC Prize 2025.
- Human "smart adult" baseline: ARC-AGI-1 ~98%, ARC-AGI-2 ~60%, with grand-prize threshold at 85% (efficient/open-source).

### ARC-AGI-1

| Date | System | Semi-Private Score | Compute / Cost |
| --- | --- | --- | --- |
| 2020 | Icecuber (Kaggle winner) | 17% | — |
| 2024 (Q1) | GPT-4o (zero-shot) | ~5% | — |
| 2024 (Q3) | Ryan Greenblatt (GPT-4o + sampling) | 42% | $/task very high |
| 2024 (Nov) | ARChitects (Kaggle 2024 winner) | 56% | — |
| 2024 (Dec) | **o3 (high efficiency)** | **75.7%** | $26/task — won ARC-AGI-Pub leaderboard |
| 2024 (Dec) | **o3 (low efficiency, 172× compute)** | **87.5%** | $4,560/task — crossed grand-prize threshold |
| 2025 (Apr) | o3 (medium, public release) | 53% | OpenAI confirmed retail-version differs from private preview |
| 2025 | o3-mini (high) / o4-mini | 34.5% / 41.8% | — |

### ARC-AGI-2

| Date | System | Score | Notes |
| --- | --- | --- | --- |
| 2025 (May) | o3 (Medium) / o3-mini / o1-pro | 0.9-3.0% | All near-zero |
| 2025 (May) | Claude 3.7 (8K) | 0.9% | — |
| 2025 (Jul) | ARC Prize 2025 Kaggle leader | ~24% (private) | Open-source focus |
| 2025 (Q4) | Grok 4 | 16% | — |
| 2025 (Nov) | GPT-5.1 | 17.6% | — |
| 2025 (Dec) | GPT-5.2 / Gemini 3 Pro Deep Think | 52.9% / 45.1% | Major jump |
| 2026 (Feb) | Claude Opus 4.6 | 68.8% | First above human baseline |
| 2026 (Mar) | GPT-5.4 | 73.3% | — |
| 2026 (Apr) | **Gemini 3.1 Pro** | **77.1%** | Top public score at the time |
| 2026 (Sep 1) | Claude Fable 5.1 | 90.0% | Anthropic system card; OpenAI's table agrees |
| 2026 (Sep 3) | **GPT-6 Astra** | **95.0%** | OpenAI launch table (Sol 92.5%, Opus 5 90.4%, Fable 5 89.2%) |

**Sources:** [ARC Prize: o3 breakthrough](https://arcprize.org/blog/oai-o3-pub-breakthrough) · [Chollet et al. ARC-AGI-2 paper](https://arxiv.org/pdf/2505.11831) · [BenchLM ARC-AGI-2](https://benchlm.ai/benchmarks/arcAgi2) · [llm-stats ARC-AGI v2](https://llm-stats.com/benchmarks/arc-agi-v2)

> **Status**: ARC-AGI-1 effectively saturated (87.5% w/ massive compute, late 2024; Astra later posted 98.5% on OpenAI's table). ARC-AGI-2 went from <3% (May 2025) to 95% (Sep 2026).

### ARC-AGI-3

Launched in 2026 as the hard successor. As of August 23 the best published score in this tracker was **7.78%** (GPT-5.6 Sol).

| Date | System | Score | Notes |
| --- | --- | --- | --- |
| 2026 (Aug) | GPT-5.6 Sol | 7.78% | Best score in the August 23 tracker |
| 2026 (Sep 3) | Claude Opus 5 | 30.2% | OpenAI launch table; Fable columns were blank |
| 2026 (Sep 3) | **GPT-6 Astra** | **99.9%** | OpenAI. ARC Prize: surpassed their human action-efficiency baseline on 96% of levels. Harness note from OpenAI: responses-API settings changed to match real-world use, not targeted at ARC-AGI-3 |

> **Status**: Fell in one release. A benchmark that was the open frontier on August 23 was saturated on September 3. Treat 99.9% as OpenAI-reported, with the harness caveat above.

---

## 9. AIME (American Invitational Mathematics Exam)

- AIME 2024 / AIME 2025 are 15-problem, integer-answer mathematics competitions used as a stress test for "reasoning" models since OpenAI's o1.

| Date | Model | AIME 2024 | AIME 2025 | Notes |
| --- | --- | --- | --- | --- |
| 2024 (Q3) | GPT-4o | 9.3% | — | AI Index 2025 |
| 2024 (Sep) | o1 | **74.4%** | ~71.5% | "IMO qualifying" gain over GPT-4o |
| 2024 (Dec) | o3 (preview) | ~87% | — | OpenAI |
| 2025 (Q1) | o3-mini (high) | — | 86.5% | Vals AI / best independent score |
| 2025 (Feb) | Grok 3 (Think, cons@64) | — | 93.3% | xAI self-report |
| 2025 (Q2) | DeepSeek R1 | — | 74-87.5% (May rev) | Open source |
| 2025 (Q2) | Gemini 2.5 Pro | — | 87.7-88% | Google |
| 2025 (Aug) | **GPT-5 (no tools)** | — | **94.6%** | OpenAI launch |
| 2025 (Aug) | GPT-5 Pro (with Python) | — | ~100% | Tool-augmented |
| 2025 (Q3) | Grok 4 | — | ~91-93% | xAI |
| 2025 (Dec) | GPT-5.2 / GPT-5.2 Pro | — | 99.0% | pricepertoken |
| 2026 (Q1) | GPT-5.2 Thinking | — | 100% | aictrl reporting |
| 2026 (Apr) | Kimi K2.5 (Reasoning) | — | 96.1% | Moonshot AI |

**Sources:** [Stanford AI Index 2025](https://hai.stanford.edu/assets/files/hai_ai-index-report-2025_chapter2_final.pdf) · [The Regularizer AIME 2025](https://www.theregularizer.com/blog/aime-2025-benchmark-results) · [IntuitionLabs AIME 2025 PDF](https://intuitionlabs.ai/pdfs/aime-2025-benchmark-an-analysis-of-ai-math-reasoning.pdf) · [pricepertoken AIME 2025](https://pricepertoken.com/leaderboards/benchmark/aime-25)

> **Status**: Closed-book saturating ~95-99%; open-book (tool-use) effectively solved. AIME 2026 problems will be needed to maintain signal.

---

## 10. FrontierMath (Epoch AI)

- Released: November 2024 (paper Dec 2024 / arXiv 2411.04872).
- Currently 350 problems: Tiers 1-3 (300 base, "undergrad to graduate") + Tier 4 (50 "research-level" added July 2025).
- Private/public split. Numbers below are on **frontiermath-2025-02-28-private (290 problems)** unless noted.

| Date | Model | Tier 1-3 Score | Tier 4 Score | Notes |
| --- | --- | --- | --- | --- |
| 2024 (Nov) | GPT-4o / Claude 3.5 / Grok 2 / Gemini 1.5 Pro / o1-preview / o1-mini | <2% | — | All initial models — paper says "no model achieved 2%" |
| 2024 (Dec) | **o3 (OpenAI internal eval)** | ~25% | — | OpenAI's announced result on the older 180-Q `frontiermath-2024-11-26` set |
| 2025 (Apr) | o3 (Epoch eval, post-release) | 18.7% | — | Lower than internal eval — different scaffold/subset |
| 2025 (Apr) | o4-mini (high) | 24.8% | — | Epoch |
| 2025 | Claude Sonnet 4.5 | 13.5% | — | — |
| 2025 (Jun) | Gemini 2.5 Pro Preview 06-05 | 10% (Epoch) / 29% later | — | — |
| 2025 (Q4) | Grok 4 | 19.7% | — | — |
| 2025 (Nov) | Claude Opus 4.5 | 20.7% | — | Epoch |
| 2025 (Dec) | **GPT-5.2** | **40.7%** | — | **Epoch resolution; matched 2025 forecast median (40%)** |
| 2026 (Feb) | Gemini 3 Pro Preview | 37.6% / 38% | 19% | Highest Tier 4 (v1 set) |
| 2026 (Mar/Apr) | GPT-5.4 | 47.6% | — | llm-stats top (v1 set) |
| 2026 (Jul, **v2 set**) | GPT-5.5 / Claude Opus 4.8 | 85.3% / 80% | 72.5% / 56.1% | From OpenAI GPT-5.6 launch table — v2 numbers not comparable to v1 rows above |
| 2026 (Jul 9, v2) | **GPT-5.6 Sol / Claude Fable 5** | **89% / 87%** | **83% / 87.8%** | Tier 4 effectively fell in mid-2026 |
| 2026 (Sep 3, v2) | **GPT-6 Astra** | — | **97.6%** | OpenAI launch table (lede says 98%). Same table: Fable 5 90.2%, Fable 5.1 87.8%, Sol 83.0%, Opus 5 73.2%. Tier 1-3 not restated |

**Sources:** [Epoch AI FrontierMath hub](https://epoch.ai/benchmarks/frontiermath/) · [arXiv 2411.04872 v7](https://arxiv.org/pdf/2411.04872) · [Epoch 2025 forecast recap](https://epoch.ai/gradient-updates/how-well-did-forecasters-predict-2025-ai-progress) · [NeoSignal FrontierMath leaderboard](https://neosignal.io/benchmarks/frontiermath-2025-02-28-private) · [llm-stats FrontierMath](https://llm-stats.com/benchmarks/frontiermath)

> **Status**: Tier 1-3 went from <2% (Nov 2024) to ~89% (Jul 2026) and was not the headline in September. Tier 4 went from ~19% on the v1 set in April 2026 to 83-88% on v2 in July, then **97.6%** (GPT-6 Astra, Sep 3). Mind the version break. On OpenAI's September table Fable 5.1 (87.8%) scores below Fable 5 (90.2%) — harness and safeguard differences, not a clean regression.

---

## 11. Humanity's Last Exam (HLE)

- Released: January 2025 by Center for AI Safety + Scale AI. ~3,000 expert-authored questions across mathematics, sciences, humanities.
- Finalized to 2,500 questions on April 3, 2025.
- Human expert ceiling estimated ~90%.

| Date | Model | Score | Notes |
| --- | --- | --- | --- |
| 2025 (Jan) | GPT-4o | 2.7% | Original release |
| 2025 (Jan) | Claude 3.5 Sonnet | 4.1% | Original release |
| 2025 (Q1) | o1 | ~8% | OpenAI |
| 2025 (Apr) | o3 (medium) / o3 (high) | 19.8% / 20.6% | OpenAI |
| 2025 (May) | Gemini 2.5 Pro Preview | 18.4-22.1% | Google |
| 2025 (Q3) | GPT-5 | 26.3% (Scale) / 35% (vendor) | — |
| 2025 (Q3) | Claude Opus 4.5 | 26.3% (Scale) / 32.1% (vendor) | — |
| 2025 (Q4) | GPT-5.1 (thinking) | 24.7% | Scale |
| 2025 (Dec) | GPT-5.2 | 28.5% (Scale) / 37% (vendor) | — |
| 2026 (Jan) | Gemini 3 Pro Preview | 37.2-37.7% | Google |
| 2026 (Feb 5) | **Claude Opus 4.6** | **40.0% (no tools) / 53.1% (with tools)** | Anthropic |
| 2026 (Mar) | GPT-5.4 (xhigh thinking) | 36.5-39% (Scale) / 41.6% (Artificial Analysis) | OpenAI |
| 2026 (Mar) | GPT-5.4 Pro | 45.3% (Scale) / 58.7% (BenchLM) | — |
| 2026 (Apr) | **Gemini 3.1 Pro Preview** | **44.7-47.3%** | Google; current Scale leader |
| 2026 (Apr) | Claude Mythos Preview | 64.7% | BenchLM (secondary report) |
| 2026 (Jul 9) | Muse Spark 1.1 | 62.1% (with tools, vendor) | Meta; led its comparison table vs Opus 4.8 (57.9) and GPT-5.5 (52.2) |
| 2026 (Aug 14) | GLM-5.3 | 62.5% (with tools, vendor) | Highest open-weights HLE score at the time; same Z.ai table puts GPT-5.6 Sol at 64.5% and Fable 5 at 63.9% with tools |
| 2026 (Sep 1) | **Claude Fable 5.1** | **60.9% no tools / 65.0% with tools** | Anthropic launch + system card. OpenAI's table agrees on 65.0% with tools |
| 2026 (Sep 3) | GPT-6 Astra | 57.2% with tools | OpenAI launch table — trails Fable 5.1, Fable 5 (63.8%), and Opus 5 (63.6%) in that same table |
| 2026 (Sep 22) | **Claude Opus 5.5** | **67.7% with tools** | Anthropic launch table. Same table revises Fable 5.1 to 65.6% and Opus 5 stays at 63.6%. Astra still 57.2% |
| 2026 (Sep 10) | DeepSeek V4.1-Flash | 36.8% (39.1% text subset); **63.9% with tools** | DeepSeek API changelog. Best confirmed open with-tools score |

**Sources:** [Scale Labs HLE leaderboard](https://scale.com/leaderboard/humanitys_last_exam_text_only) · [aictrl: Reasoning Race](https://aictrl.dev/blog/reasoning-benchmarks) · [pricepertoken HLE](https://pricepertoken.com/leaderboards/benchmark/hle) · [BenchLM HLE](https://benchlm.ai/benchmarks/hle)

> **Status**: Partially solved. With-tools scores moved from a 60-64.5% cluster in August to 65.0% (Fable 5.1, Sep 1) and then **67.7%** (Opus 5.5, Sep 22). Astra, the model that saturated ARC-AGI-3 and FrontierMath Tier 4, scores 57.2% here on OpenAI's own table. The gap to the ~90% human-expert ceiling is still about 22 points on the with-tools number.

---

## 12. MMMU (Multimodal Massive Multi-task Understanding)

- Released: November 2023 (paper); evaluations widely reported from January 2024.
- 11,500 college-exam multimodal questions across 30 subjects. Best human expert ~88.6%, lower bound ~76.2%.
- **MMMU-Pro** (Sep 2024): harder vision-only/augmented variant.

### MMMU (original)

| Date | Model | Score | Notes |
| --- | --- | --- | --- |
| 2023 (Dec) | Gemini 1.0 Pro / GPT-4V | 47.9% / 56.8% | Original paper baselines |
| 2024 (May) | GPT-4o | 69.1% | OpenAI |
| 2024 (Jun) | Claude 3.5 Sonnet | 68.3% | Anthropic |
| 2024 (Sep) | o1 | 78.2% (AI Index) | OpenAI; 4.4 pt below human |
| 2025-2026 | o4-mini (high) / GPT-5 | 79.1-79.2% | Saturating original benchmark |
| 2026 (Apr) | Top of original MMMU | ~79.2% | pricepertoken |

### MMMU-Pro

| Date | Model | Score | Notes |
| --- | --- | --- | --- |
| 2024 (Q4) | GPT-4o (Pro) | 51.9% | Original paper |
| 2025 (Q2) | Claude 3.5 / Gemini 1.5 Pro | ~50-55% | — |
| 2025 (Q4) | GPT-5 / Claude Opus 4.5 | 76-80% | — |
| 2026 (Feb) | Gemini 3 Pro | 81.0-87.5% | Google (Vals AI vs vendor) |
| 2026 (Feb 26) | **Gemini 3.1 Pro Preview** | **88.21%** | Vals AI — within 0.4 pt of human ceiling |
| 2026 (Apr) | GPT-5.4 Pro | 94% | BenchLM (vendor) |
| 2026 (Apr) | Claude Mythos Preview | 92.7% | BenchLM (secondary) |

**Sources:** [MMMU paper 2023](https://arxiv.org/abs/2311.16502) · [Vals AI MMMU/MMMU-Pro](https://www.vals.ai/benchmarks/mmmu) · [llm-stats MMMU-Pro](https://llm-stats.com/benchmarks/mmmu-pro) · [BenchLM MMMU-Pro](https://benchlm.ai/benchmarks/mmmuPro) · [Stanford AI Index 2025](https://hai.stanford.edu/assets/files/hai_ai-index-report-2025_chapter2_final.pdf)

> **Status**: Original MMMU saturated ~79%. MMMU-Pro at human-ceiling — Vals AI calls it "approaching asymptotic limit".

---

## 13. LiveCodeBench

- Released: March 2024 (Jain et al., arXiv 2403.07974). Continuously refreshed competitive programming problems from LeetCode/Codeforces/AtCoder, post-training-cutoff.
- The most contamination-resistant mainstream coding benchmark.

| Date | Model | Score | Notes |
| --- | --- | --- | --- |
| 2024 (Mar) | GPT-4-turbo / Claude 3 Opus | Top of original eval | Best across most scenarios |
| 2024 (Q4) | GPT-4o / Claude 3.5 Sonnet | Mid-50s % | Aggregator-reported |
| 2025 (Q3) | GPT-5 series | 70-80% | OpenAI |
| 2025 (Q4) | GPT-5.1 / Claude Opus 4.5 | 75-80% | — |
| 2026 (Feb) | GPT-5.2 Codex | 87.99% | Vals AI |
| 2026 (Mar) | GPT-5.3 Codex | 87.31% (Vals) / 85% (BenchLM) | — |
| 2026 (Feb 26) | **Gemini 3.1 Pro Preview** | **88.49%** | Vals AI — current top |

**LiveCodeBench Pro (April 2026):** GPT-5.4 87.5% · Gemini 3.1 Pro 82.9% · Muse Spark 80.0% · Grok 4.20 74.2% · Claude Opus 4.6 70.7%.

**Sources:** [LiveCodeBench paper / homepage](https://livecodebench.github.io/index.html) · [Vals AI LiveCodeBench](https://www.vals.ai/benchmarks/lcb) · [BenchLM contamination-free post](https://benchlm.ai/blog/posts/livecodebench-contamination-free) · [BenchLM LiveCodeBench Pro](https://benchlm.ai/benchmarks/liveCodeBenchPro)

> **Status**: Approaching saturation on the easy/medium splits. Hard splits still discriminate meaningfully. Pro variant has 17-point top-10 spread and remains the best contamination-resistant signal.

---

## 14. Chatbot Arena Elo (lmarena.ai / LMSYS)

- Crowdsourced anonymous side-by-side preference voting; relative Elo rating, no fixed ceiling.
- Started May 2023 by LMSYS; rebranded Arena/lmarena.ai.

| Month | #1 Model | Elo | Crown change? |
| --- | --- | --- | --- |
| 2023 (May) | GPT-4 | 1225 | First leaderboard |
| 2023 (Dec) | GPT-4-0314 | ~1240 | OpenAI |
| 2024 (Feb) | GPT-4-0125-preview | 1251 | OpenAI |
| 2024 (Mar) | Claude 3 Opus | ~1260 | First Anthropic #1 |
| 2024 (Apr) | GPT-4-Turbo-2024-04-09 | 1275 | OpenAI back |
| 2024 (May) | GPT-4o-2024-05-13 | 1302 | OpenAI |
| 2024 (Sep) | chatgpt-4o-latest | ~1320 | OpenAI |
| 2025 (Jan) | o1-2024-12-17 | ~1420 | First reasoning model #1 |
| 2025 (Mar) | grok-3-preview-02-24 | ~1450 | First xAI #1 |
| 2025 (Jul) | gemini-2.5-pro | ~1461 | Google |
| 2025 (Q4) | Claude Opus 4.5 (thinking) | ~1468 | Anthropic |
| 2026 (Feb) | **claude-opus-4-6-thinking** | **1500** | Anthropic; first 1500 Elo |
| 2026 (Mar) | gpt-5.4-high | ~1495-1518 (week-to-week #1) | OpenAI |
| 2026 (Apr) | **gemini-3.1-pro-preview** | 1487-1537 | Google |
| 2026 (Apr 20) | Top cluster (Claude Opus 4.6/4.7, Gemini 3.1 Pro, Muse Spark, GPT-5.4-high) | 1472-1505 | 5-way tie |

**Total movement:** Vicuna-13B at 1094 (May 2023) → 1500+ (April 2026) = **+406 Elo in 37 months** (~11 pts/month). Crown changed hands 21 times. OpenAI #1 for 16 of 37 months (43%); Google 7 months; Anthropic 5 months.

**Sources:** [BenchLM LLM Leaderboard History](https://benchlm.ai/llm-leaderboard-history) · [LMSYS original Week 4 post (2023)](https://lmsys.org/blog/2023-05-25-leaderboard/) · [OpenLM.ai Arena+](https://openlm.ai/chatbot-arena) · [lmarena.ai](https://lmarena.ai)

> **Status**: No saturation — relative ranking. But criticism of "stylistic preference" and contamination led to the Arena adding category-specific Elos (coding, vision, math, hard prompts) and the AAII (Artificial Analysis Intelligence Index) as composite ranking.

---

## Meta-pattern: how benchmarks die

### A. The standard saturation curve

For benchmarks released as "hard" between **2020 and 2023**, the typical trajectory has been:

- **Year 0**: SOTA at 25-50% (often near random for multiple-choice). Headline "this benchmark will hold for years".
- **Year 1**: Frontier doubles, but still well below human.
- **Year 2**: Crosses human-expert baseline (the moment the benchmark stops being a frontier signal).
- **Year 3**: Top cluster within 2-3 pp; differences are within inter-run noise.
- **Year 4+**: Successor benchmark emerges with harder questions or harder format.

| Benchmark | Hard → saturated | Years |
| --- | --- | --- |
| MMLU | 43.9% (2020) → 92% (2024) | ~4 |
| HumanEval | 28.8% (2021) → 96% (2024) | ~3 |
| GSM8K | ~20% (2021) → 97% (2024) | ~3 |
| MATH | ~7% (2021) → 97% (2024-25) | ~4 |
| BBH | ~50% (2022) → 94% (2025-26) | ~3 |
| GPQA Diamond | 39% (2023) → 94% (2026) | ~2.5 |
| ARC-AGI-1 | <5% (2024 GPT-4o) → 87.5% (Dec 2024 o3 high-compute) | ~1 (with reasoning models) |
| MMMU | 47.9% (2023) → 79% (2025-26) | ~2 |
| SWE-bench Verified | 22% (2024) → 80%+ (2026) | ~1.5 |

### B. Saturation has accelerated

Median time-to-saturation:

- **Pre-2022 benchmarks** (MMLU, GSM8K, MATH, HumanEval): 3-4 years.
- **2023 benchmarks** (GPQA, MMMU): 2-2.5 years.
- **2024 benchmarks** (SWE-bench Verified, FrontierMath Tier 1-3, ARC-AGI-1 semi-private): 1-2 years.
- **2025 benchmarks** (HLE, ARC-AGI-2, FrontierMath Tier 4): partially solved within ~1 year.

The drivers of the acceleration:

1. **Reasoning-model paradigm** (o1 in Sep 2024). The single biggest jump in benchmark history: +34.5 MATH, +26.7 GPQA, +65.1 AIME 2024 over GPT-4o, all from one architecture pattern (extended chain-of-thought + RL).
2. **Test-time compute scaling**. o3's ARC-AGI-1 result (87.5% at 172× compute) demonstrated that compute can buy benchmark scores. Cost-per-task entered the conversation: ARC Prize started measuring "intelligence per dollar".
3. **Tool use blurs categories**. AIME 2025: closed-book ~95%, with-Python ~100%. FrontierMath, HLE: with-tool scores 10-20 pp above no-tool scores.
4. **Data contamination is real**. By 2026, multiple aggregators flag MMLU, HumanEval, MATH, GSM8K as contaminated. LiveCodeBench, FrontierMath, ARC-AGI-2 specifically designed to resist.

### C. Categorization as of September 2026

**Saturated (>=90%, ceiling effects, no longer differentiates):**

- MMLU · HumanEval · GSM8K · MATH · BBH · GPQA Diamond (96.0%, GPT-6 Astra) · MMMU (original) · ARC-AGI-1 · ARC-AGI-2 (95.0%, Astra) · ARC-AGI-3 (99.9%, Astra — was 7.8% in August) · AIME 2024 · AIME 2025 (closed-book ~95%, tools ~100%) · FrontierMath Tier 4 v2 (97.6%, Astra) · SWE-bench Verified (vendor-reported ≥88%; contamination flagged).

**Mostly solved (frontier ≥75%, discriminates weakly):**

- FrontierMath Tier 1-3 (top ~89%) · MMMU-Pro (top 88-94%, near human ceiling) · LiveCodeBench (top 88%) · Terminal-Bench 2.1 (top ~92% ultra; six labs within ~1pp at 87-89 standard) · BrowseComp (top ~92%) · SWE-bench Pro vendor-scaffold (81.2%, Fable 5.1).

**Partially solved (~25-75%, frontier still climbs visibly):**

- HLE (with tools 67.7% Opus 5.5; Fable 5.1 65.6% in the same table; Astra 57.2% on OpenAI's table; open 63.9% DeepSeek V4.1-Flash) · OSWorld 2.0 (Opus 5.5 81.8% partial) · GDPval-AA v2.1 (Opus 5.5 1846 Elo; this is a new version — Fable 5.1's 1853 was on v2) · Terminal-Bench 4.0 (Opus 5.5 66.4% at xhigh, Astra 57.9% at high, Gemini 3.8 Flash 19.1%) · Terminal-Bench 3.0 (top 34.6% Sol; open 30.0% V4.1-Flash) · SWE Marathon · Agents' Last Exam (Astra 59.3% on OpenAI's table; DeepSeek 31.8%).

**Still hard:**

- BBEH · long-horizon autonomy where the new terminal and science benches still spread labs by tens of points (Terminal-Bench Science: Astra 64.6%, Fable 5.1 52.6%, Sol 22.4%) · standardized SWE-bench Pro (~59% on the earlier Scale setup).

### D. What the open thread *isn't* solving yet

By September 23, 2026, no AI system reliably:

- Leads every board at once. Astra saturated ARC-AGI-3, FrontierMath Tier 4, and ExploitBench. Opus 5.5 leads Terminal-Bench 4.0 and HLE with tools, and still trails Astra on Terminal-Bench Science (58.7% vs 64.6%). Astra trails Fable 5.1 on the Artificial Analysis Intelligence Index v4.1.1 (61.2 vs 65.7); Opus 5.5 has no published AA Index number yet.
- Reaches the ~90% human-expert estimate on Humanity's Last Exam. The best with-tools number is 67.7%.
- Wins ARC Prize *Grand Prize* terms (85% on ARC-AGI-2 with high-efficiency, open-source). Closed models are at 95%; the openness and cost constraints are the remaining gate.
- Shows decisive Chatbot Arena dominance — no new Arena crown was verified for this update; the spring 2026 cluster was a five-way tie around 1500.
- Puts a cheap Flash-tier model on Terminal-Bench 4.0. Gemini 3.8 Flash scores 19.1% there against 73.7% on DeepSWE.

### E. Successor benchmark map

| Saturated → | Successor (year) |
| --- | --- |
| MMLU → | MMLU-Pro (2024) → AAII / GPQA-Diamond / HLE |
| HumanEval → | LiveCodeBench (2024) / SWE-bench Verified (2024) → SWE-bench Pro / Terminal-Bench 2 (2025) → Terminal-Bench 3.0 (Jul 2026) |
| GSM8K → | MATH → AIME → FrontierMath (2024) |
| BBH → | BBEH (Feb 2025) |
| MMMU → | MMMU-Pro (Sep 2024) → multimodal+grounded composite |
| ARC-AGI-1 → | ARC-AGI-2 (Mar 2025) |
| Chatbot Arena Elo → | Category Elos + AAII composite |

---

## Sources & evaluation aggregators (canonical)

- **Original benchmark papers**: Hendrycks 2020 (MMLU), Chen 2021 (HumanEval), Cobbe 2021 (GSM8K), Hendrycks 2021 (MATH), Suzgun 2022 (BBH), Rein 2023 (GPQA), Jimenez 2023 (SWE-bench), Yue 2023 (MMMU), Jain 2024 (LiveCodeBench), Glazer/Epoch 2024 (FrontierMath), CAIS 2025 (HLE), Chollet et al. 2025 (ARC-AGI-2).
- **Stanford AI Index 2025 ch.2** — definitive 2020-2024 benchmark progress: https://hai.stanford.edu/assets/files/hai_ai-index-report-2025_chapter2_final.pdf
- **Epoch AI** — FrontierMath and forecasting: https://epoch.ai/benchmarks/frontiermath/ · https://epoch.ai/gradient-updates/how-well-did-forecasters-predict-2025-ai-progress
- **ARC Prize** — ARC-AGI: https://arcprize.org/blog/oai-o3-pub-breakthrough · https://arxiv.org/pdf/2505.11831
- **Anthropic SWE-bench post**: https://www.anthropic.com/research/swe-bench-sonnet
- **Vals AI** — independent reproductions: https://www.vals.ai/benchmarks
- **Scale Labs** — HLE official leaderboard: https://scale.com/leaderboard/humanitys_last_exam_text_only
- **lmarena.ai / OpenLM.ai** — Chatbot Arena Elo: https://openlm.ai/chatbot-arena
- **Aggregators** (with caveats): BenchLM (https://benchlm.ai), pricepertoken (https://pricepertoken.com), llm-stats (https://llm-stats.com), llmdb (https://llmdb.com), BenchGecko (https://benchgecko.ai), LM Market Cap (https://lmmarketcap.com), TokenMix (https://tokenmix.ai), TokenCalculator (https://tokencalculator.com), IntuitionLabs (https://www.intuitionlabs.ai).

---

*Last updated: September 23, 2026 (GPT-6 Astra saturates ARC-AGI-3 and FrontierMath Tier 4; Claude Opus 5.5 then takes Terminal-Bench 4.0 and HLE with tools; DeepSeek V4.1-Flash; Kimi K2.8 Preview has no public scores). Previous update: August 23, 2026.*
