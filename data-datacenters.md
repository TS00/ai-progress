# AI Datacenter & Compute Buildout: 2020 → September 2026

*Compiled April 26, 2026. Updated September 23, 2026 for NVIDIA Q2 FY27 and the sites/chips that moved. Numbers marked **(est.)** are analyst/Epoch AI estimates rather than disclosed figures; **(disclosed)** are from earnings or official filings; **(reported)** are from credible press without primary-source confirmation.*

## Update — September 23, 2026

- **NVIDIA Q2 FY27** (quarter ended July 26, reported August 26): revenue **$96.2B**, datacenter **$89.0B** (+18% QoQ, +117% YoY). Q3 guide **$108B ±2%**, with no China datacenter compute revenue assumed. GAAP/non-GAAP gross margin 75.0% in the quarter. Source: [NVIDIA Q2 FY27 release](https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-Announces-Financial-Results-for-Second-Quarter-Fiscal-2027/default.aspx).
- **Vera Rubin is in full production**, with racks at CoreWeave, Google Cloud, Microsoft Azure, Oracle Cloud, and Nebius. CFO Colette Kress: Vera Rubin about **20% of datacenter revenue in Q3**. NVIDIA content per gigawatt: Hopper ~$18B, Grace Blackwell ~$25B, **Vera Rubin ~$40B** (CPU + GPU + NVLink + networking).
- **H200-to-China did not become a business.** The same filing: licensed H200 shipments were **under 1% of datacenter revenue**; a **$0.4B** charge in the first half of FY27 for excess H200 inventory. NVIDIA says PRC restrictions kept it from selling all the chips it had licenses for.
- **Stargate Norway** (and a UK site) were reported paused. Korea JoongAng (Sep 7, 2026): OpenAI and Nscale did not finalize a Norway offtake, and Microsoft took the project over. Stargate Korea, a year after the Samsung/SK letters of intent, still had no settled site, power, or funding.
- Training-compute leadership is unchanged in public FLOP estimates: Grok 4 at ~5×10²⁶ remains the largest *disclosed* run. The new qualitative datapoint is OpenAI's: VP of research Aidan Clark told Fortune that GPT-6 Astra was the first OpenAI pretrain on more than 100,000 GPUs, at Stargate in Texas.

---

## TL;DR — what changed in six years

- **Training compute at the frontier scaled ~10,000× from 2020 to 2025.** GPT-3 (May 2020) was trained on ~3×10²³ FLOP. Grok 4 (mid-2025), the largest known run, used ~5×10²⁶ FLOP. Epoch AI clocks the trend at **~5× per year** for frontier language models since 2020 (doubling every ~5.2 months).
- **NVIDIA datacenter revenue went from $6.7B in FY21 to $193.7B in FY26** — a 29× increase in five years. FY26 GPU shipments are dominated by Blackwell (B200/GB200/GB300), which crossed Hopper in mid-2025 and is "sold out" through 2026.
- **The Big Four hyperscalers (MSFT, GOOG, META, AMZN) are guiding to ~$635–665B of 2026 capex**, up from ~$155B in 2022. Adding Oracle pushes the Big Five to **$660–690B** for 2026.
- **The first multi-GW single-site AI campuses are operational.** xAI's Colossus (Memphis) hit ~2 GW and ~555k GPUs in Jan 2026. AWS/Anthropic Project Rainier (Indiana) is live with ~500k Trainium2 chips at 2.2 GW. Stargate Abilene is at 0.6 GW operational, scaling to 1.2 GW.
- **US data-center electricity use roughly doubled 2018→2023** (76 → 176 TWh, 4.4% of US electricity). The IEA put the 2025 share at ~7%; LBNL projects 325–580 TWh (6.7–12% of US electricity) by 2028.
- **Hyperscalers contracted >10 GW of new US nuclear capacity in 2024–25** — Three Mile Island restart for Microsoft, Kairos SMRs for Google, X-energy/Susquehanna for Amazon, plus a Meta 1–4 GW RFP.
- **Compute is geographically concentrated**: Epoch AI estimates the US holds ~74.5% of tracked AI cluster performance, China ~14.1%, EU ~4.8% (May 2025). Five hyperscalers (MSFT/GOOG/META/AMZN/ORCL) own ~71% of global AI compute by Q4 2025 (up from 63% in Q1 2024).
- **Export controls tightened, eased on paper, and then failed to produce a trade.** April 2025 ban on H20 to China cost NVIDIA ~$8B in Q2 FY26 outlook. A Jan 2026 BIS rule moved H200/MI325X to case-by-case review with a 25% revenue fee. By the July 2026 quarter, licensed H200 shipments were under 1% of NVIDIA datacenter revenue.

---

## 1. Training compute evolution

### 1.1 Trend

Epoch AI's "[Training compute of frontier AI models grows by 4-5× per year](https://epoch.ai/blog/training-compute-of-frontier-ai-models-grows-by-4-5x-per-year)" is the canonical reference. Their key figures (updated April 2026):

| Metric (frontier language models, since 2020) | Value | 90% CI |
|---|---|---|
| Training-compute growth rate | **5× per year** | 4× to 6× |
| Doubling time | 5.2 months | 4.6–6.0 months |
| Cost-per-training-run growth | 3.5× per year | 2.8–4.4× |
| Largest known training run | **5×10²⁶ FLOP (Grok 4)** | — |
| AI chip FLOP/s per dollar | 1.37× per year | — |
| Global AI compute capacity doubling | **~7 months** | (~3.3×/year since 2022) |

> Source: [epoch.ai/trends](https://epoch.ai/trends) and [ml-progress.com](https://ml-progress.com/), updated Apr. 8, 2026.

### 1.2 Frontier training runs by year

Best public estimates (most are **(est.)** unless otherwise noted). Sources: Epoch AI [model-counts post](https://epoch.ai/data-insights/models-over-1e25-flop), [GPT-5 estimate](https://www.linkedin.com/posts/epochai_we-recently-wrote-that-gpt-5-is-likely-the-activity-7382145618284032000-8Q5E).

| Year | Largest known model | Developer | Training FLOP (est.) | Notes |
|---|---|---|---|---|
| 2020 | GPT-3 (davinci, 175B) | OpenAI | **3.1 × 10²³** | First "modern" frontier run |
| 2021 | Megatron-Turing NLG 530B / Gopher | MS-NV / DM | ~3 × 10²³ | A100 era |
| 2022 | PaLM 540B | Google | ~2.5 × 10²⁴ | TPU v4 |
| 2023 (Mar) | GPT-4 | OpenAI | **2.1 × 10²⁵** | ~15–25k A100s, several months |
| 2023 (Dec) | Gemini Ultra 1.0 | Google | **5.0 × 10²⁵** | TPU v5p |
| 2024 (May) | GPT-4o | OpenAI | 3.8 × 10²⁵ | Multimodal omni |
| 2024 (mid) | Llama 3 405B | Meta | ~4 × 10²⁵ | 16k H100s |
| 2024 (Q4) | Claude 3.5 Opus / GPT-4.5 | Anthropic / OpenAI | 1–2 × 10²⁶ (speculative) | First "next-gen" runs |
| 2025 (Feb) | **Grok-3** | xAI | **4.6 × 10²⁶** | Colossus 100k+ H100s |
| 2025 (Mar) | GPT-4.5 | OpenAI | 6.4 × 10²⁵ (Epoch low-precision est.) | |
| 2025 (mid) | **Grok 4** | xAI | **~5 × 10²⁶** *(largest known)* | |
| 2025 (Aug) | GPT-5 | OpenAI | **~5 × 10²⁵** (est., pretrain ~3e25 + RL) | First mainline GPT below predecessor in pure compute |
| 2025–26 | Claude Opus 4 / 4.5 | Anthropic | 1–2 × 10²⁶ (speculative) | Run on AWS Trainium2 + GCP TPUs |
| 2025–26 | Gemini 2.5 / 3 Pro | Google | speculative; not imputed by Epoch | TPU Trillium / Ironwood |

**Key inflection**: Epoch projects **~10 models above 10²⁶ FLOP by start of 2026, ~30 by 2027, >200 by 2030** under their median scenario; the first frontier *open-weight* model crossed 10²⁶ FLOP in late 2025 ([Epoch](https://epoch.ai/data-insights/open-models-threshold)).

### 1.3 Cluster sizes used for training

Reported peak GPU counts for major training runs (rough, from press + Epoch):

| Model | Year | Cluster GPUs (peak, est.) | Notes |
|---|---|---|---|
| GPT-3 | 2020 | ~10k V100 | Microsoft Azure |
| GPT-4 | 2023 | 10–25k A100 | "Microsoft Azure supercomputers" |
| Llama 3.1 405B | 2024 | 16k H100 | Meta RSC clusters |
| Grok 3 | 2025 | ~100k H100 | Colossus 1, Memphis |
| GPT-5 | 2025 | 25–80k H100-eq (est.) | Microsoft Azure (CometAPI estimate, not disclosed) |
| Claude (Opus 4 / 4.5) | 2025–26 | hundreds of thousands of TPU + Trainium2 | Project Rainier |

---

## 2. GPU & accelerator deployment

### 2.1 NVIDIA datacenter revenue (annual, fiscal year ending late Jan)

Source: NVIDIA 10-K / press releases via [stockanalysis.com](https://stockanalysis.com/stocks/nvda/metrics/data-center-revenue/) and [ycharts](https://ycharts.com/indicators/nvidia_corp_nvda_data_center_revenue).

| Fiscal year (ends ~Jan) | Datacenter revenue | YoY |
|---|---|---|
| FY2020 (Jan 2020) | $2.98B | — |
| FY2021 (Jan 2021) | $6.70B | +124% |
| FY2022 (Jan 2022) | $10.61B | +58% |
| FY2023 (Jan 2023) | $15.00B | +41% |
| FY2024 (Jan 2024) | **$47.52B** | +217% |
| FY2025 (Jan 2025) | **$115.19B** | +142% |
| FY2026 (Jan 2026) | **$193.74B** | +68% |

Quarterly (most recent full year, then the new year): Q1 FY26 $39.1B → Q2 FY26 $41.1B → **Q3 FY26 $51.2B** → Q4 FY26 ~$62B (implied). **Q2 FY27 datacenter revenue: $89.0B** (disclosed, quarter ended July 26, 2026). Source: [NVIDIA Q3 FY26 release](https://nvidianews.nvidia.com/_gallery/download_pdf/691e34d93d633290a88deeef/), [NVIDIA Q2 FY27 release](https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-Announces-Financial-Results-for-Second-Quarter-Fiscal-2027/default.aspx).

### 2.2 NVIDIA datacenter GPU shipments (units)

Mix of TechInsights, Omdia, and Epoch AI estimates. Most numbers are **(est.)**.

| Year | Units shipped (M) | Mix highlight | Source |
|---|---|---|---|
| 2022 | 2.64 | A100-dominant | TechInsights via [HPCwire](https://www.hpcwire.com/2024/06/10/nvidia-shipped-3-76-million-data-center-gpus-in-2023-according-to-study/) |
| 2023 | **3.76** (98% market share) | H100 ramp; ~500k–650k H100 alone | TechInsights |
| 2024 | ~4–5 (est.) | H100/H200 dominant; first GB200 samples Q4 | Omdia/analyst |
| 2025 | ~6–7 (est.) | H200 + Blackwell ramp; **~13k Blackwell samples Q3FY25 → ~200k Q3FY26 → ~500k Q4FY26** | NVIDIA earnings |
| 2026 (proj.) | "Sold out" — backlog reportedly 3.6M Blackwell GPUs | GB200/GB300 + first Vera Rubin late 2026 | iBuidl / SemiAnalysis |

Per-unit ASP for B200: $30,000–$40,000 ([iBuidl Q4 FY25 analysis](https://ibuidl.org/blog/nvidia-q4-2025-earnings-analysis-20260310)).

**Cumulative installed AI accelerator base.** Epoch AI: as of end-2025, the world has **~20 million H100-equivalents** of compute (Stargate's planned 9 GW alone could power that much). Five hyperscalers own ~71% (Q4 2025).

### 2.3 NVIDIA architecture timeline

| Architecture | Generation | First shipped | Notes |
|---|---|---|---|
| Ampere | A100 | mid-2020 | Trained GPT-3, GPT-4, original Llama |
| Hopper | H100 (80/94 GB) | Q3 2022 (volume Q1 2023) | Backbone of 2023–2024 frontier |
| Hopper refresh | H200 (141 GB HBM3e) | Q3 2024 | "Fastest-ramping product in NVIDIA history" |
| Ada (consumer) | (not DC) | — | — |
| Hopper-China | H800 / H20 (export-compliant) | 2023 / 2024 | H20 banned to China April 2025, partial unblock Jan 2026 |
| Blackwell | B100 / B200 / GB200 NVL72 | first samples Q3 FY25 (Oct 2024); volume mid-2025 | $30–40k ASP; CoWoS-L packaging |
| Blackwell Ultra | B300 / GB300 | mid-late 2025 | Used in Colossus 2 and Stargate phase-2 |
| Vera Rubin | R100 / VR200 | **full production, August 2026** (was "sampling 2026, volume 2027") | Racks at CoreWeave, GCP, Azure, OCI, Nebius. ~20% of Q3 FY27 datacenter revenue guided. ~$40B NVIDIA content per GW |

> "Anthropic will run and scale on NVIDIA infrastructure, initially adopting **1 gigawatt of compute capacity with NVIDIA Grace Blackwell and Vera Rubin systems**" — [NVIDIA Q3 FY26 release](https://nvidianews.nvidia.com/_gallery/download_pdf/691e34d93d633290a88deeef/).

### 2.4 Custom silicon

| Vendor | Chip | First deployed | 2025–26 status |
|---|---|---|---|
| Google | TPU v4 | 2021 | Trained PaLM, early Gemini |
| Google | TPU v5e / v5p | 2023–2024 | Mainstream production through 2024 |
| Google | **TPU v6e "Trillium"** | GA Dec 16, 2024 | Trained Gemini 2.0; 4.7× v5e perf |
| Google | **TPU v7 "Ironwood"** | GA late Nov 2025; v7x GA Mar 31, 2026 | 9,216-chip pods, 1.77 PB shared HBM, 9.6 Tb/s ICI; Anthropic to use **up to 1M Ironwood TPUs** |
| Google | TPU v8 (8t / 8i) | Announced Cloud Next 2026 | Ships later in 2026 |
| AWS | Trainium / Inferentia | 2022 | Modest uptake |
| AWS | **Trainium2** | 2024 (volume late 2024) | **~500k chips at Project Rainier (Indiana)** in Oct 2025; 1M+ by end-2026 |
| AWS | Trainium3 | Dec 2025 sampling, 2026 volume | Co-designed with Anthropic |
| Microsoft | Maia 100 | Nov 2023 | First-gen, 700W |
| Microsoft | **Maia 200** | Launched Jan 26, 2026 | 3 nm TSMC, 144B transistors, 216 GB HBM3e, ~10.2 PFLOPS FP4; deployed in Iowa & Phoenix; powers GPT-5.2 + Copilot |
| Meta | MTIA v1/v2 | 2023–2024 | Internal ranking + GenAI |
| Meta | MTIA v3+ | 2025 | Hundreds of thousands deployed; Meta also taking AWS Trainium capacity (CoreWeave deal, Apr 2026) |

> By late-2025 industry analysis, custom accelerators process **>50% of hyperscaler internal inference workloads**; NVIDIA's hyperscaler share fell from ~90% to ~75% ([Microsoft blog](https://blogs.microsoft.com/blog/2026/01/26/maia-200-the-ai-accelerator-built-for-inference/)).

---

## 3. Major datacenter projects & clusters

### 3.1 Headline AI campuses

| Campus | Owner / partner | Location | Power (current → planned) | GPUs / chips | Status (Apr 2026) | Source |
|---|---|---|---|---|---|---|
| **Colossus 1 + 2 + "MACROHARDRR"** | xAI | Memphis, TN + Southaven, MS | ~2 GW (1 GW live, +500 MW Building 3 in build) | **~555,000 GPUs** (mostly GB200/GB300; ~30k legacy H100/H200) | Operational; targeting 1M GPUs late 2026 | [Introl](https://introl.com/blog/xai-colossus-2-gigawatt-expansion-555k-gpus-january-2026) |
| **Stargate – Abilene, TX** ("Project Ludicrous") | OpenAI/Oracle/Crusoe | Abilene, TX | **0.6 GW live → 1.2 GW Q3 2026** (8 buildings, 4M sq ft, 1,000+ acres) | ~500k H100-equivalents live; up to 400k GB200s planned | 4 of 8 buildings online; 2.1 GW expansion **canceled** Q1 2026 (Microsoft/Meta taking adjacent 900 MW) | [Epoch](https://epochai.substack.com/p/openai-stargate-where-the-us-sites), [ConstructionOwners](https://www.constructionowners.com/news/stargate-ai-data-center-nears-completion-in-abilene) |
| Stargate – other US sites | OpenAI / SoftBank / Oracle | Shackelford TX, Doña Ana NM, Lordstown OH, Milam County TX, Wisconsin, Michigan | Combined ~7+ GW planned; total **9+ GW by 2029** | TBD | All 7 US sites under active construction; Milam fast-build steel up; total $450B+ committed of $500B | Same as above |
| **Project Rainier** | AWS for Anthropic | New Carlisle, IN (St. Joseph County) | **2.2 GW** (7 of 30 buildings online; 1,200 acres; 6M sq ft) | **~500k Trainium2** today → 1M by end-2026 (largest non-NVIDIA cluster) | Operational Oct 2025; "largest known deployment of non-NVIDIA compute anywhere" | [Amazon](https://www.aboutamazon.com/news/aws/aws-project-rainier-ai-trainium-chips-compute-cluster), [CNBC](https://www.cnbc.com/2025/10/29/amazon-opens-11-billion-ai-data-center-project-rainier-in-indiana.html) |
| Anthropic-Amazon expansion | Amazon / Anthropic | Multi-site | **Up to 5 GW** total Trainium2/3/4 commitment | nearly 1 GW Trainium2/3 by end-2026 | Announced; multi-year through Trainium4 | [Anthropic](https://www.anthropic.com/news/anthropic-amazon-compute) |
| **Hyperion** | Meta | Richland Parish, LA (Holly Ridge / Franklin Farm) | **2 GW phase-1 (2026–27) → 5 GW by ~2030** | NVIDIA Blackwell + AMD MI450 | Under construction (since Mar 2026 ground-break); 2,250 acres, 4M sq ft, $10B initial / $27–30B JV w/ Blue Owl + PIMCO | [Wikipedia](https://en.wikipedia.org/wiki/Hyperion_(data_center)), [Meta](https://datacenters.atmeta.com/richland-parish-data-center/) |
| Prometheus | Meta | New Albany, OH / multiple | 1+ GW (planned) | TBD | Announced 2025 |
| Anthropic – 1 GW NVIDIA deal | Anthropic / NVIDIA | TBD | 1 GW Grace-Blackwell + Vera Rubin | TBD | Announced Q3 FY26 (Oct/Nov 2025) — Anthropic's first NVIDIA infrastructure adoption |
| **Solstice** | DOE / Oracle / NVIDIA | Argonne (?) | TBD | **100,000 Blackwell GPUs** (DOE's largest AI supercomputer) | Announced Q3 FY26 |
| **Equinox** | DOE / Oracle / NVIDIA | TBD | TBD | 10,000 Blackwell GPUs | Announced Q3 FY26 |
| CoreWeave fleet | CoreWeave | 32 datacenters globally | 360 MW (early 2025) → **850 MW under contract end-2025** | **250,000 GPUs** end-2024; rapidly expanding GB200 NVL72 + GB300 | $87.8B revenue backlog; Meta added $21B/Dec-2032 commitment Apr 2026 | [NextPlatform](https://www.nextplatform.com/2025/03/05/coreweaves-250000-strong-gpu-fleet-undercuts-the-big-clouds/) |
| Crusoe Abilene | Crusoe / Oracle / Microsoft | Abilene, TX (also adjacent 900 MW for MSFT) | 1.2 GW | hosts Stargate's GB200 racks | Phase 1 live 2025; named DCD "North American Data Center Project of the Year" 2025 | [Crusoe](https://www.crusoe.ai/resources/newsroom/crusoe-wins-north-american-data-center-project-of-the-year-at-2025-data-center-dynamics-global-awards) |
| MS Mt. Pleasant, WI; Quincy, WA; Phoenix; Des Moines IA | Microsoft | Multiple US | ~2 GW added in 2025 alone; >400 facilities globally | Mix; **Maia 200 deployed in Des Moines + Phoenix** | $80B FY25 capex on AI DCs; reported $80B in unfilled Azure orders for lack of power | [Introl](https://introl.com/blog/hyperscaler-capex-690-billion-microsoft-azure-power-bottleneck-2026) |
| Susquehanna campus | Amazon | Salem Township, PA | 960 MW (next to Susquehanna nuclear plant) | TBD | $20B+ committed, 15 buildings on 1,600 rezoned acres |
| **Stargate UAE** | OpenAI / G42 / Oracle / NVIDIA / Cisco / SoftBank | Abu Dhabi | **1 GW** (200 MW phase 1 Q3 2026, full by 2028, +2 GW under consideration) | TBD | First international Stargate; first OpenAI-for-Countries partnership | [OpenAI](https://openai.com/index/introducing-stargate-uae/) |
| Stargate Norway | OpenAI / Nscale / Aker → reported Microsoft | Norway | 230 MW (+290 MW expansion option) | 100,000 NVIDIA GPUs had been planned by end-2026 | **Paused.** Korea JoongAng, Sep 7, 2026: offtake not finalized; project taken over by Microsoft. A UK site was also reported paused |
| Stargate Argentina | OpenAI / Sur Energy | Patagonia | up to 500 MW | TBD | $25B LOI, RIGI incentive regime |
| Stargate UK / EU AI Gigafactories | OpenAI + EU | various | TBD | TBD | Early-stage; MOUs only |

### 3.2 Other notable buildouts

- **Google**: Council Bluffs IA, Pryor OK, Lenoir NC, Henderson NV, Mesa AZ, multiple TPU v5p / Trillium / Ironwood pods. Cloud backlog $240B end-Q3 2025 (+55% sequentially). 2026 capex $175–185B; CEO: 60% on servers (TPU/GPU/CPU), 40% data centers + networking.
- **Microsoft**: $80B FY25 spend; ~2 GW added in 2025 alone; over 400 facilities globally. The 900 MW Abilene parcel adjacent to Stargate is now Microsoft's after the Stargate expansion fell through. CEO Nadella: "GPUs sit idle; we lack the electricity to install them" — $80B unfulfilled Azure orders.
- **Oracle**: 4.5 GW agreement with OpenAI; $50B 2026 capex guide; building Solstice and Equinox DOE machines with NVIDIA.

### 3.3 Single-site power records

| Year | Largest single AI campus (live) | Power |
|---|---|---|
| 2022 | Microsoft Azure GPT-4 cluster | ~30–60 MW (est.) |
| 2023 | Meta RSC, Microsoft Phoenix | ~150 MW |
| 2024 (Jul) | xAI Colossus 1 (100k H100) | 150 → 250 MW |
| 2024 (Q4) | Colossus expanded to 200k GPUs | ~420 MW |
| 2025 (Q4) | Project Rainier 7 of 30 buildings | ~700 MW |
| 2026 (Jan) | **Colossus 1+2+MACROHARDRR**: 555k GPUs | **~2 GW** |
| 2026 (Q3 target) | **Stargate Abilene** full 8 buildings | 1.2 GW |
| 2030 (target) | Meta Hyperion full buildout | 5 GW |

---

## 4. Capex, power, and power deals

### 4.1 Hyperscaler capex (Big Five: AMZN, GOOG, META, MSFT, ORCL)

Source: [Introl Jan 2026 capex tracker](https://introl.com/blog/hyperscaler-capex-690-billion-microsoft-azure-power-bottleneck-2026), Yahoo/CNBC ([Big Tech 2026 capex](https://www.cnbc.com/2026/02/06/google-microsoft-meta-amazon-ai-cash.html)).

| Year | Big Four (MSFT/GOOG/META/AMZN) | Big Five (+ ORCL) | YoY (Big Five) | AI share |
|---|---|---|---|---|
| 2020 | ~$120B (est.) | ~$125B | — | small |
| 2021 | ~$135B | ~$140B | — | small |
| 2022 | $156B | ~$160B | +14% | growing |
| 2023 | $144B | ~$150B | -6% | rising |
| 2024 | **$229B** | **$256B** | +63% | majority |
| 2025 | **$381B** (Yahoo) / $360B (other) | **$443B** | +73% | ~70% AI |
| **2026 (guide)** | **$635–665B** | **$660–690B** | +55% | ~75% (~$450–500B AI) |

**Per-company 2026 guidance** (announced Q4 2025 / Q1 2026 earnings):

| Company | 2026 capex guide | 2025 actual | YoY |
|---|---|---|---|
| Amazon | **$200B** | $125B (est.) / $100B (other) | +60–100% |
| Alphabet | **$175–185B** | $91.4B | ~+100% |
| Meta | **$115–135B** | $66–72B | +60–87% |
| Microsoft | **~$120–145B** | ~$80–95B | +30–50% |
| Oracle | **$50B** | ~$35B | +43% |

Free-cash-flow casualties: **Amazon projected -$17 to -$28B FCF in 2026** (Morgan Stanley/BofA); Alphabet FCF -90% to ~$8.2B (Pivotal); Meta FCF -90% (Barclays). Big-Five raised **$108B in debt in 2025** alone (vs. $32B/yr historical avg.); Morgan Stanley/JPM project $1.5T tech-sector debt issuance over coming years. Alphabet priced a $20B 7-part bond Feb 9, 2026, including a 100-year sterling tranche.

Capital intensity (capex/revenue) is at historic highs: AWS 57%, Meta 52%, MSFT 48%, GOOG 45% — vs. 10–25% historic norms.

### 4.2 US data-center electricity consumption

Sources: [LBNL 2024 report](https://eta-publications.lbl.gov/sites/default/files/2024-12/lbnl-2024-united-states-data-center-energy-usage-report.pdf), [EPRI](https://epri.co/dc-electricity-growth), [EIA](https://www.eia.gov/todayinenergy/detail.php?id=67344), IEA.

| Year | US DC electricity (TWh) | % of US electricity | Source |
|---|---|---|---|
| 2014 | ~60 | ~1.5% | LBNL |
| 2018 | 76 | 1.9% | LBNL |
| 2023 | **176** | **4.4%** | LBNL |
| 2024 | 177–192 (est.) | ~5% | EPRI |
| 2025 | ~250 (est.); IEA pegs share at **~7%** | ~7% | IEA |
| 2028 (LBNL) | **325–580** | **6.7–12%** | LBNL low/high |
| 2030 (EPRI) | **380–790** | **9–17%** | EPRI |

Growth rate: 7%/yr (2014–18) → 18%/yr (2018–23) → projected 13–27%/yr (2023–28). DCs accounted for **~50% of all US electricity demand growth in 2025** per IEA. EIA's STEO sees ERCOT load up ~10%/yr 2025–27, PJM ~3%/yr.

### 4.3 Gigawatt+ campuses announced (US, ≥1 GW planned)

| Project | Owner | Planned GW | Status |
|---|---|---|---|
| Colossus (Memphis + Southaven) | xAI | ~2 GW (toward 1M GPUs / >2 GW) | Live |
| Project Rainier | AWS/Anthropic | 2.2+ GW | Live (Phase 1) |
| Hyperion | Meta | 2 GW → **5 GW** | Construction |
| Stargate Abilene | OpenAI/Oracle | 1.2 GW | 0.6 GW live |
| Stargate Milam County | OpenAI/SoftBank | 1.2 GW | Under construction |
| Stargate (5 other US sites) | OpenAI | 5+ GW combined | Active dev |
| Stargate UAE | OpenAI/G42 | 1 GW | 200 MW Q3 2026 |
| Susquehanna campus | Amazon | up to 1+ GW | Build-out |
| Solaris (xAI proposal) | xAI | 1.1 GW (2027) | Permitting |
| MS Mt. Pleasant + others | Microsoft | multiple, GW-scale | Operational |

**Power as constraint.** Microsoft has reported **$80B in unfulfilled Azure orders** ascribed to lack of electricity. Both Amazon's Indiana site and xAI's Memphis campus rely heavily on **gas turbines + Tesla Megapacks** for on-site generation to bypass utility interconnect queues (xAI: 35 mobile turbines, 420 MW; 208 Megapacks; permits expire 2027).

### 4.4 Nuclear deals (10+ GW contracted in 12 months)

Source: [Introl Dec 2025](https://introl.com/blog/nuclear-power-ai-data-centers-microsoft-google-amazon-2025).

| Hyperscaler | Counterparty | Capacity | Tech | Status |
|---|---|---|---|---|
| **Microsoft** | Constellation Energy | 835 MW (Three Mile Island Unit 1, renamed "Crane Clean Energy Center") | Existing PWR restart | 20-yr PPA, $1.6B restart, $1B DOE loan (closed); target 2027–28 |
| **Google** | Kairos Power | up to 500 MW (6–7 SMRs) | Molten-salt KP-FHR | First reactor 2030; full 500 MW by 2035; Hermes 2 first 50 MW via TVA |
| **Amazon** | Talen Energy / Susquehanna | 960 MW (existing PWR) | $20B campus next to plant | Build-out |
| **Amazon** | X-Energy | 5 GW SMR target (Xe-100) | $500M Series C; Energy Northwest 320–960 MW | Through 2039 |
| **Amazon** | Dominion Energy | ~300 MW SMR | MOU at North Anna VA | Exploratory |
| **Meta** | RFP | 1–4 GW (SMR + large) | Various | RFP issued; Constellation IL plant PPA in place |
| **Oracle/OpenAI** (Stargate) | TBD | "SMRs planned for baseload" | — | Conceptual |

---

## 5. Global distribution & export controls

### 5.1 Geography of AI compute

Epoch AI's GPU Clusters dataset ([epoch.ai/data-insights/ai-supercomputers-performance-share-by-country](https://epoch.ai/data-insights/ai-supercomputers-performance-share-by-country)) — covers ~10–20% of global AI-oriented compute as of March 2025.

| Country / region | Share of AI cluster performance (May 2025) |
|---|---|
| **United States** | **74.5%** |
| **China** | **14.1%** |
| EU-27 (combined) | 4.8% |
| Norway | 1.8% |
| Japan | 1.4% |

**China caveat**: China stopped Top500 submissions after 2017. China's MIIT claimed ~230 EFLOPS of national capacity by July 2024 (target 300 by 2025); Top500 reports only 0.281 EFLOPS — an enormous "dark compute" pool largely on Huawei Ascend + grey-market H100/A100. Sanchez's [State of Global AI Compute 2025](https://www.sanchez.vc/geocoded-special-reports/state-of-global-ai-compute-2025-edition) estimates ~850k H100-equivalents in the US fleet end-2025 vs. ~100k in China and ~50k in EU — though Chinese figures here exclude Huawei Ascend.

### 5.2 Hyperscaler concentration

Source: [Epoch AI hyperscaler share](https://epoch.ai/data-insights/hyperscalers-control-most-compute).

| Period | MSFT+GOOG+META+AMZN+ORCL share of global AI compute |
|---|---|
| Q1 2024 | 63% |
| Q4 2025 | **71%** |

Industry's share of global AI compute (vs. governments/academia): **40% in 2019 → ~80% in 2025** (Epoch AI [trends](https://epoch.ai/blog/trends-in-ai-supercomputers)).

### 5.3 Export controls timeline

Sources: [IAPS](https://www.iaps.ai/research/bis-licensing-policy-for-h200s), [Introl AI OVERWATCH analysis](https://introl.com/blog/bis-h200-china-export-policy-ai-overwatch-act-2026), [Tech-Insider](https://tech-insider.org/nvidia-h200-chip-sales-china-2026/).

| Date | Action |
|---|---|
| Oct 2022 | Biden initial BIS controls (no advanced GPU/equipment to China) |
| Oct 2023 | Tightening: closes A800/H800 loophole; introduces TPP + bandwidth thresholds; NVIDIA forced to design **H20** |
| Jan 2025 | "AI diffusion framework" (export tiers) under outgoing Biden |
| **Apr 2025** | Trump admin **bans H20 to China** → NVIDIA $4.5B Q1 charge, **$8B Q2 FY26 revenue impact** |
| **Jan 13–15, 2026** | BIS Federal Register rule **2026-00789**: H200 + AMD MI325X moved from "presumption of denial" to **case-by-case review** with **25% revenue fee** to US gov't. Cap = 50% of cumulative US sales (~850k–900k H200-eq). Chips must pass US-based independent testing |
| **Jan 21, 2026** | House Foreign Affairs **AI OVERWATCH Act** advances 42–2 → 2-yr Blackwell ban, congressional veto over export licenses |
| **Feb 2026** | State Department **blocks** all H200 shipments pending review; China grants conditional approval for ~400k of 2M ordered |
| **Mar 2026** | NVIDIA stops producing China-specific chips; Beijing restricts purchases to "special circumstances" |
| **Aug 26, 2026** | NVIDIA Q2 FY27 filing: licensed **H200 shipments <1% of datacenter revenue**; **$0.4B** H1 FY27 charge for excess H200 inventory. Company says it could not sell all licensed H200s because of PRC restrictions, and assumes **no China datacenter compute revenue** in the Q3 outlook |

**Net effect**: Chinese frontier labs (DeepSeek, Alibaba Qwen, Moonshot Kimi, ByteDance Doubao) train primarily on grey-market H100/H800 inventories, H20, and **Huawei Ascend 910C** (Huawei plans 600k 910C shipments in 2026 regardless of US action). The January 2026 case-by-case H200 opening did not turn into volume: by the July quarter it was a rounding error in NVIDIA's datacenter revenue. The binding control on the next models is no longer only the chip license. September's releases shipped with trusted-access lanes for cyber and biology (Anthropic Life Sciences Verification, Google Fairwind, OpenAI's Critical-tier safeguards on GPT-6 Astra, SpaceXAI's invite-only Grok 4.7 red team).

---

## 6. Selected sources

- **Epoch AI** — [trends dashboard](https://epoch.ai/trends), [4-5×/yr post](https://epoch.ai/blog/training-compute-of-frontier-ai-models-grows-by-4-5x-per-year), [model count thresholds](https://epoch.ai/blog/model-counts-compute-thresholds), [open-models 1e26 threshold](https://epoch.ai/data-insights/open-models-threshold), [country shares](https://epoch.ai/data-insights/ai-supercomputers-performance-share-by-country), [hyperscaler share](https://epoch.ai/data-insights/hyperscalers-control-most-compute), [GPT-5 estimate](https://www.linkedin.com/posts/epochai_we-recently-wrote-that-gpt-5-is-likely-the-activity-7382145618284032000-8Q5E), [Stargate site tracker](https://epochai.substack.com/p/openai-stargate-where-the-us-sites)
- **NVIDIA** — [FY25 annual report](https://s201.q4cdn.com/141608511/files/doc_financials/2025/annual/NVIDIA-2025-Annual-Report.pdf), [Q2 FY26](https://nvidianews.nvidia.com/_gallery/download_pdf/68af69043d6332f1d02dec91/), [Q3 FY26](https://nvidianews.nvidia.com/_gallery/download_pdf/691e34d93d633290a88deeef/)
- **TechInsights / HPCwire** — [3.76M datacenter GPU shipments 2023](https://www.hpcwire.com/2024/06/10/nvidia-shipped-3-76-million-data-center-gpus-in-2023-according-to-study/)
- **Introl Blog** — [Colossus 2 GW](https://introl.com/blog/xai-colossus-2-gigawatt-expansion-555k-gpus-january-2026), [Memphis Colossus history](https://introl.com/blog/xai-memphis-colossus-100000-gpu-supercomputer-infrastructure), [Stargate $500B](https://introl.com/blog/openai-stargate-500-billion-ai-infrastructure-2025), [Project Rainier](https://dcpulse.com/project/aws-project-rainier-indiana-11-billion-ai-supercluster), [hyperscaler capex](https://introl.com/blog/hyperscaler-capex-690-billion-microsoft-azure-power-bottleneck-2026), [nuclear deals](https://introl.com/blog/nuclear-power-ai-data-centers-microsoft-google-amazon-2025), [BIS H200 policy](https://introl.com/blog/bis-h200-china-export-policy-ai-overwatch-act-2026)
- **Amazon / AWS** — [Project Rainier activation](https://www.aboutamazon.com/news/aws/aws-project-rainier-ai-trainium-chips-compute-cluster), [Anthropic 5 GW expansion](https://www.anthropic.com/news/anthropic-amazon-compute)
- **Meta** — [Hyperion announcement](https://datacenters.atmeta.com/richland-parish-data-center/), [Wikipedia Hyperion](https://en.wikipedia.org/wiki/Hyperion_(data_center))
- **Microsoft** — [Maia 200 launch](https://blogs.microsoft.com/blog/2026/01/26/maia-200-the-ai-accelerator-built-for-inference/)
- **Google** — [Trillium GA Dec 2024](https://cloud.google.com/blog/products/compute/introducing-trillium-6th-gen-tpus), [Ironwood GA Nov 2025](https://cloud.google.com/blog/products/compute/ironwood-tpus-and-new-axion-based-vms-for-your-ai-workloads), [TPU release notes](https://docs.cloud.google.com/tpu/docs/release-notes)
- **OpenAI** — [Stargate UAE](https://openai.com/index/introducing-stargate-uae/), [Stargate Norway](https://openai.com/index/introducing-stargate-norway), [Stargate Argentina coverage (BNamericas)](https://www.bnamericas.com/en/features/argentina-joins-openais-stargate-project-with-a-500mw-megadata-center)
- **CNBC** — [Project Rainier](https://www.cnbc.com/2025/10/29/amazon-opens-11-billion-ai-data-center-project-rainier-in-indiana.html), [Ironwood unveiling](https://www.cnbc.com/2025/11/06/google-unveils-ironwood-seventh-generation-tpu-competing-with-nvidia.html), [$700B 2026 capex](https://www.cnbc.com/2026/02/06/google-microsoft-meta-amazon-ai-cash.html)
- **Power / energy** — [LBNL 2024 DC report](https://eta-publications.lbl.gov/sites/default/files/2024-12/lbnl-2024-united-states-data-center-energy-usage-report.pdf), [EPRI](https://epri.co/dc-electricity-growth), [EIA STEO](https://www.eia.gov/todayinenergy/detail.php?id=67344), [Constellation/TMI restart](https://www.utilitydive.com/news/doe-loan-constellation-crane-nuclear-restart/805923/), [Kairos/Google](https://www.datacenterfrontier.com/energy/article/55235902/google-and-amazon-make-major-inroads-with-smrs-to-bring-nuclear-energy-to-data-centers)
- **Export controls** — [IAPS H200 analysis](https://www.iaps.ai/research/bis-licensing-policy-for-h200s), [BIS rule 2026-00789](https://introl.com/blog/bis-h200-export-policy-china-case-by-case-controversy-2026)
- **Stargate Abilene reporting** — [Texas Monthly Feb 2026](https://www.texasmonthly.com/news-politics/abilene-stargate-artificial-intelligence/), [Bloomberg/Yahoo Finance cancellation](https://finance.yahoo.com/news/openais-massive-stargate-data-center-154932400.html)
- **Geographic shares** — [Sanchez & Co. State of Global AI Compute 2025](https://www.sanchez.vc/geocoded-special-reports/state-of-global-ai-compute-2025-edition)

---

*Generated 2026-04-26. This document compiles ranges and estimates from multiple secondary sources; for any number that drives a decision, verify directly against the linked primary source. Compute estimates from Epoch AI carry ±0.5–1 OOM uncertainty for closed models. Hyperscaler capex figures are official guidance for 2026 and may move with quarterly earnings.*
