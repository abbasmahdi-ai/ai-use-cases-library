# 📚 AI Use Cases Library

The **AI Use Cases Library** is an open, curated collection of real-world **AI implementation case studies**.  
It contains thousands of examples of how AI is applied across industries, enriched with consistent taxonomy, tools, and outcomes.



---

## 📊 Dataset Overview

- **Final dataset**: 2,260 curated use cases (`/data/use-cases.csv`)  
- **In-Review dataset**: 266 cases pending validation (`/in-review/use-cases-in-review.csv`)  
- **Excluded dataset**: 690 cases that did not meet criteria (`/excluded/use-cases-excluded.csv`)  
- **Total considered**: 3,216 cases  

Every case has a permanent **CaseID**:
- Final: `aicase-00001` → `aicase-02260`  
- In-Review: `aicase-02261` → `aicase-02526`  
- Excluded: `aicase-x0001` → `aicase-x0690`  


<br />

👉 In addition to the main dataset, feel free to **browse the in-review and excluded datasets**.  
They provide useful context on cases that are being validated or did not meet inclusion criteria, and help illustrate the curation process behind the library.

⚠️ **Disclaimer**: The `in-review` and `excluded` datasets are **not production quality**.  
They contain incomplete information, missing enrichment, or non-AI cases. You can view them for background reference only.

---

## 📂 Repository Structure

```text
ai-use-case-library/
├── data/                  # Final curated dataset + schema
├── in-review/             # Cases pending review
├── excluded/              # Cases that did not make the cut
├── docs/                  # Taxonomy, methodology, contributing guidelines
├── insights/              # Trends & vendor analysis (v1.0)
├── awesome-lists/         # Curated lists (featured cases in v1.0)
├── tools/                 # Example notebook, (future: search UI)
├── charts/                # Industry, vendor, and outcomes visuals
├── ROADMAP.md             # Future plans
├── CHANGELOG.md           # Version history
├── CASEID_POLICY.md       # CaseID assignment rules
├── LICENSE
└── README.md
````

---

## 🎯 Goals
- Provide a **central reference** of AI use cases across industries.
- Support **learning, research, and training** with real examples.
- Encourage **responsible adoption** of generative AI.
- Enable **community contributions** for continuous enrichment.


---

## 🚀 Quick Start

1. **Explore the dataset**

   * [Final dataset](data/use-cases.csv) (2,260 curated cases)
   * [Schema](data/schema.md) (field definitions)
   * [Taxonomy](docs/taxonomy.md)
   * [Methodology](docs/methodology.md)

2. **View insights**

   * [Trends analysis](insights/trends-analysis.md)
   * [Vendor comparison](insights/vendor-comparison.md) 
   * *(Planned: [Industry breakdowns](insights/industry-breakdown.md) — see [ROADMAP](ROADMAP.md))*

   

3. **See curated highlights**

   * [Featured cases](awesome-lists/featured-cases.md)

4. **Run example analysis**

   * [Analysis notebook](tools/analysis-scripts/analysis_notebook.ipynb)

5. **Check visuals**

   - [Charts Gallery](./charts/charts.md) → browse all visuals in one page
   - Individual charts:
     - [Industry distribution](./charts/industry_distribution.png)  
     - [Domain distribution](./charts/domain_distribution.png)  
     - [Outcomes breakdown](./charts/outcomes_breakdown.png)  
     - [Vendor distribution (tools)](./charts/vendor_by_tools.png)  
     - [Vendor distribution (source)](./charts/vendor_by_source.png)  
   - ➡️ More in the [charts folder](./charts/)  

   > **Note on Vendor Presence**  
      > Vendor comparisons in this repository are based on the *share of documented case studies in our dataset (2,260 cases)*.  
      >  - **Tool/Technology mentions** reflect where vendor products (e.g., Azure, Copilot, GPT, Claude) appear in implementations.  
      > - **Source (Publisher)** indicates who published the case study (e.g., Microsoft, AWS).  
      >
   > These numbers show relative presence in documented cases, **not actual global adoption**. Vendors with larger publication pipelines may appear overrepresented.


6. **Tools & Scripts**
   - [Starter analysis notebook](./tools/analysis-scripts/analysis_notebook.ipynb) → quick demo of loading and analyzing the dataset
   - [requirements.txt](./tools/analysis-scripts/requirements.txt) → minimal dependencies (`pandas`, `matplotlib`)
   - See [tools/analysis-scripts/](./tools/analysis-scripts/) for details

---

## 🤝 Contributing & Suggestions

We welcome **corrections and new use case suggestions**.
To keep data quality high, all contributions flow through the **in-review dataset** first.

* Suggest a **new use case** → use the [New Use Case issue template](.github/ISSUE_TEMPLATE/new-use-case.yml).
* Report an error or update → use the [Correction issue template](.github/ISSUE_TEMPLATE/correction.yml).
* Please do **not** submit direct PRs editing the datasets (`use-cases.csv`, `in-review/`, or `excluded/`).

<br>

See [docs/contributing.md](docs/contributing.md) for details.

---

## 🗺️ Roadmap

* v1.0 includes: datasets, schema/docs, trends & vendor insights, featured cases, analysis notebook, charts.
* v1.1+ will expand with industry breakdowns, curated lists by domain/industry, and interactive search/exploration.

See [ROADMAP.md](ROADMAP.md) for details.

---

## 📜 License

Released under the [MIT License](LICENSE).
You are free to use, share, and adapt the dataset with attribution.

---

## 🙌 Acknowledgments

This project was built to promote **AI literacy and transparency**.
It is actively maintained and will continue to evolve with new sources, taxonomy refinements, and community contributions.