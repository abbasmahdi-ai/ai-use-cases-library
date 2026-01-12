# AI Use Cases Library

The most comprehensive open dataset of real-world enterprise AI implementations - **3,023 documented use cases** showing how AI is transforming industries.

**Key Findings**: Google Gemini capturing 24% of deployments | Reasoning models (o1/o3) emerging for expert-level tasks | Healthcare breakthroughs in drug discovery | AI expanding into manufacturing

---

## Dataset Overview

- **3,023 curated use cases** across 20+ industries
- **99.97% data completeness** maintained
- **11+ major AI vendors** documented
- **Updated January 2026**

Every case has a permanent **CaseID**: `aicase-00001` → `aicase-03132`

<br />

👉 In addition to the main dataset, feel free to **browse the in-review and excluded datasets**.  
They provide useful context on cases that are being validated or did not meet inclusion criteria, and help illustrate the curation process behind the library.

⚠️ **Disclaimer**: The `in-review` and `excluded` datasets are **not production quality**.  
They contain incomplete information, missing enrichment, or non-AI cases. You can view them for background reference only.

---

## Repository Structure

```text
ai-use-cases-library/
├── data/                  # Final curated dataset + schema
├── in-review/             # Cases pending review (78 cases)
├── excluded/              # Cases that did not meet criteria (720 cases)
├── docs/                  # Taxonomy, methodology, contributing guidelines
├── insights/              # Trends & vendor analysis
├── awesome-lists/         # Curated lists (featured cases)
├── tools/                 # Analysis notebook, scripts
├── charts/                # Industry, vendor, and outcomes visuals
├── ROADMAP.md             # Future plans
├── CHANGELOG.md           # Version history
├── CASEID_POLICY.md       # CaseID assignment rules
├── LICENSE
└── README.md
```

---

## Goals

- Provide a **central reference** of AI use cases across industries
- Support **learning, research, and training** with real examples
- Track **emerging trends** in AI adoption and technology maturity
- Enable **community contributions** for continuous enrichment
- Document **breakthrough applications** that push the boundaries of what's possible

---

## Quick Start

### 1. **Explore the dataset**

   * [Final dataset](data/use-cases.csv) (**3,023 curated cases**)
   * [Schema](data/schema.md) (field definitions)
   * [Taxonomy](docs/taxonomy.md)
   * [Methodology](docs/methodology.md)

### 2. **View insights**

   * [**Trends analysis**](insights/trends-analysis.md) - 7 major trends from 3,023 cases
     - Reasoning models: The next leap (o1/o3/GPT-5)
     - Agentic AI going mainstream
     - Healthcare: From support to discovery
     - Climate & sustainability impact
     - Multimodal & voice AI breakthroughs
     - Autonomous systems at scale
   
   * [**Vendor comparison**](insights/vendor-comparison.md) - Competitive landscape analysis
     - Google's explosive growth with Gemini
     - Microsoft's enterprise dominance
     - OpenAI's innovation leadership
     - Anthropic's quality-focused approach
     - AWS Bedrock's multi-model flexibility
   
   * [**Featured cases**](awesome-lists/featured-cases.md) - 50+ breakthrough applications
     - Novel applications (4-hour bacterial diagnosis, brain-to-speech)
     - Healthcare breakthroughs (drug discovery, rapid diagnostics)
     - Financial inclusion (tax filing for 200K+ gig workers)
     - Climate solutions (precision agriculture, carbon removal)

### 3. **Check visuals**

   - [**Charts Gallery**](./charts/charts.md) → browse all visuals in one page
   - Individual charts:
     - [Industry distribution](./charts/industry_distribution.png) - Top 20 industries
     - [Domain distribution](./charts/domain_distribution.png) - Top 18 functional domains
     - [Outcomes breakdown](./charts/outcomes_breakdown.png) - 8 outcome categories
     - [Vendor adoption by tools](./charts/vendor_by_tools.png) - 7 major vendors
     - [Vendor presence by publisher](./charts/vendor_by_source.png) - 7 top sources
   - ➡️ More in the [charts folder](./charts/)  

   > **Note on Vendor Presence**  
   > Vendor comparisons in this repository are based on the *share of documented case studies in our dataset (3,023 cases)*.  
   >  - **Tool/Technology mentions** reflect where vendor products (e.g., Azure, Copilot, GPT, Claude, Gemini) appear in implementations.  
   > - **Source (Publisher)** indicates who published the case study (e.g., Microsoft, AWS, Google).  
   >
   > These numbers show relative presence in documented cases, **not actual global adoption**. Vendors with larger publication pipelines may appear overrepresented.

### 4. **Run example analysis**

   * [Analysis notebook](tools/analysis-scripts/analysis_notebook.ipynb)
   * [Requirements](tools/analysis-scripts/requirements.txt) - minimal dependencies (`pandas`, `matplotlib`)
   * See [tools/analysis-scripts/](./tools/analysis-scripts/) for details

---

## Key Statistics

### Dataset Metrics
| Metric | Value |
|--------|-------|
| **Total Cases** | 3,023 |
| **Data Completeness** | 99.97% |
| **Industries Covered** | 20+ major industries |
| **Functional Domains** | 18+ domains |
| **Vendors Documented** | 11+ major AI providers |
| **Organizations** | 1,953+ unique companies |

### Top Categories
| Category | Leader | Count |
|----------|--------|-------|
| **#1 Industry** | Technology | 492 cases (16.3%) |
| **#1 Domain** | Operations & Supply Chain | 413 cases (13.7%) |
| **#1 Outcome** | Time savings/Speed | 1,302 cases (43.1%) |
| **#1 Specific Tool** | Google Gemini | 405 mentions |
| **#1 Vendor (Tools)** | Microsoft | 767 cases (25.4%) |
| **#1 Publisher** | Google | 996 cases (33.0%) |

---

## Featured Highlights

### Breakthrough Applications
- **Biofy Technologies**: 4-hour bacterial diagnosis (vs 5 days), saving 2,000 lives/year
- **University of Michigan**: Intraoperative brain tumor diagnosis during surgery
- **ClearTax**: 200,000+ blue-collar workers filed taxes independently, unlocking 300M INR in refunds
- **Law&Company**: 6,000 lawyers (20% of South Korea) adopted AI platform in 180 days
- **cubic**: 60x faster code review (2 minutes vs 2 hours)

### Healthcare Innovation
- **Exscientia**: AI-designed molecules in clinical trials, 10x fewer compounds needed, 80% cost reduction
- **NHS Grampian**: 12% increase in breast cancer detection, notification time cut from 14 to 3 days
- **Innoplexus**: AI-driven drug discovery pipeline for neurodegenerative diseases
- **A-Alpha Bio**: 12x increase in protein-binding prediction throughput

### Climate & Sustainability
- **John Deere**: 70% reduction in chemical use through precision agriculture
- **Microsoft Research**: Discovered new battery chemistry with 70% less lithium
- **Charm Industrial**: AI-accelerated carbon sequestration
- **Avanade**: AI "talking to trees" for plant health monitoring

### Enterprise Scale
- **Klarna**: 2.3M conversations in first month (equivalent to 700 full-time agents)
- **BBVA**: 2,900 custom GPTs deployed in 5 months, 83% employee adoption
- **Nubank**: Serves 114M customers, 70% reduction in Tier 1 chat times
- **Mercado Libre**: AI operations equivalent to 9,000 human operators

---

## Contributing & Suggestions

We welcome **corrections and new use case suggestions**.
To keep data quality high, all contributions flow through the **in-review dataset** first.

* Suggest a **new use case** → use the [New Use Case issue template](.github/ISSUE_TEMPLATE/new-use-case.yml)
* Report an error or update → use the [Correction issue template](.github/ISSUE_TEMPLATE/correction.yml)
* Please do **not** submit direct PRs editing the datasets (`use-cases.csv`, `in-review/`, or `excluded/`)

<br>

See [docs/contributing.md](docs/contributing.md) for details.

---

## Roadmap

### Current Capabilities
✅ 3,023 curated cases across industries  
✅ Comprehensive trends and vendor analysis  
✅ 5 publication-ready charts  
✅ Enhanced classification taxonomy  
✅ Featured breakthrough applications  

### Near-Term (v2.1)
🎯 Industry deep-dives (Healthcare, Manufacturing, Finance, Retail)  
🎯 Technology-specific analysis (Reasoning models, Agentic AI, Multimodal)  
🎯 Expanded awesome lists (by technology, by outcome)  
🎯 Interactive search tool  

### Medium-Term (v2.5+)
🚀 Target 4,000+ cases  
🚀 Geographic expansion (APAC, EMEA, LATAM)  
🚀 Interactive dashboard  
🚀 Enhanced vendor coverage  
🚀 Advanced analytics capabilities  

See [ROADMAP.md](ROADMAP.md) for complete roadmap and release timeline.

---

## License

Released under [MIT and CC-BY-4.0 Licenses](LICENSE).
You are free to use, share, and adapt the dataset with attribution.

---

## Citation

If you use this dataset in research or publications, please cite:

```
AI Use Cases Library. (2026). 
Retrieved from https://github.com/abbasmahdi-ai/ai-use-cases-library
```

---

## Quick Links

- **Dataset**: [use-cases.csv](data/use-cases.csv) | [Schema](data/schema.md) | [Taxonomy](docs/taxonomy.md)
- **Insights**: [Trends](insights/trends-analysis.md) | [Vendors](insights/vendor-comparison.md) | [Featured Cases](awesome-lists/featured-cases.md)
- **Visuals**: [Charts Gallery](charts/charts.md) | [Analysis Notebook](tools/analysis-scripts/analysis_notebook.ipynb)
- **Community**: [Contributing](docs/contributing.md) | [Roadmap](ROADMAP.md) | [Changelog](CHANGELOG.md)

---

## Version History & Updates

<details>
<summary><b>What's New in v2.0</b> (January 2026) - Current Release</summary>

### Major Achievements
- **+763 new cases** (+34% growth)
- **Data quality**: Maintained 99.97% completeness despite significant growth
- **Enhanced taxonomy**: 4-field classification system for improved accuracy

### Key Findings
- **Google Gemini surge**: +77% adoption (409 → 724 tool mentions)
- **Reasoning models emerging**: +135% growth (20 → 47 cases using o1/o3/GPT-5)
- **Manufacturing expansion**: +50% cases (100 → 150), showing AI moving beyond digital sectors
- **Healthcare innovation**: 347 cases (up from 280) spanning drug discovery to diagnostics
- **Agentic AI mainstream**: 358 cases of multi-agent systems in production

### Breakthrough Applications
- 4-hour bacterial diagnosis (Biofy Technologies)
- Intraoperative brain tumor detection (U. Michigan)
- Tax filing for 200K+ blue-collar workers (ClearTax)
- 60x faster code review cycles (cubic)
- AI "talking to trees" for sustainability (Avanade)

### Updated Content
- ✅ Trends analysis - 7 major trends documented
- ✅ Vendor comparison - Competitive dynamics and market shifts
- ✅ Featured cases - 50+ breakthrough applications
- ✅ All charts - 5 publication-ready visualizations
- ✅ Analysis notebook - Updated for 3,023 cases

See [CHANGELOG.md](CHANGELOG.md) for complete v2.0 release notes.

</details>

<details>
<summary><b>Previous Versions</b></summary>

### v1.0 (Initial Release)
- 2,260 curated use cases
- Core taxonomy and schema established
- Initial trends and vendor analysis
- 5 baseline charts

</details>

---

## Acknowledgments

This project was built to promote **AI literacy and transparency**.  

The library is actively maintained and will continue to evolve with new sources, taxonomy refinements, and community contributions.

---

**Current Version**: v2.0 (January 2026) - 3,023 use cases documented and growing!
