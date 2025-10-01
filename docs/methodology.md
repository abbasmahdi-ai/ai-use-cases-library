# 📖 Methodology – AI Use Cases Library

This document explains how the AI Use Cases Library dataset was built, normalized, and maintained.  
It is intended to provide **transparency**, **reproducibility**, and **guidance** for future contributions.

---

## 1. 🔍 Sources
We collected use cases from a wide range of **primary and secondary sources**, including:
- Official vendor case study portals (OpenAI, Anthropic, IBM, Nvidia, AWS, Google, Microsoft, etc.)
- Customer success stories from vendor blogs
- Press releases and news articles (cross-verified where possible)
- Academic and research papers (for edge or experimental use cases)
- Company reports and whitepapers

---

## 2. 📦 Collection Process
- Automated scraping tools were used where allowed (with respect for robots.txt).  
- Manual collection was performed for sources with restricted or blocked scraping.  
- Each entry was captured with **organization, title, description, URL, and source vendor** as the minimal fields.

---

## 3. 🧹 Cleaning & Normalization
- Removed duplicates across vendors and overlapping case studies.  
- Filtered out "AI-washing" (cases labeled *AI-powered* but lacking any AI/ML component).  
- Consolidated fragmented descriptions into a **normalized structure** with clear fields:
  - **Organization**
  - **Use Case Title**
  - **Description**
  - **Industry / Subindustry**
  - **Domain**
  - **Tools / Technologies**
  - **Outcomes & Benefits**
  - **Source URL**

---

## 4. 🏷 Taxonomy Assignment
Each case was tagged using a custom taxonomy (see [`docs/taxonomy.md`](taxonomy.md)) across:
- **Industry** (e.g., Healthcare, Financial Services, Manufacturing)  
- **Subindustry Tags** (e.g., Pharmaceuticals, Insurance, Automotive)  
- **Domain** (e.g., Customer Experience, HR, Risk & Compliance)  
- **Outcomes** (e.g., cost savings, efficiency, innovation, customer engagement)  
- **Tools & Technologies** (where specified, e.g., ChatGPT, Azure OpenAI Service, Claude, Amazon Bedrock, NVIDIA NeMo)

---

## 5. 🧩 Enrichment
- Used **LLM-based enrichment scripts** to:
  - Suggest better descriptive titles  
  - Expand vague descriptions into clearer summaries  
  - Standardize industry/domain mapping  
  - Tag missing outcomes/benefits
- Manual review was applied for quality assurance.

---

## 6. 🚫 Exclusions
Cases were excluded if:
- They contained **no real AI/ML component** (pure analytics, BI, or automation only)  
- The **source URL was broken** or insufficiently documented  
- The description was **too vague** (e.g., “improved efficiency with AI” with no detail)  

These are documented in [`excluded/use-cases-excluded.csv`](../excluded/).

---

## 7. 📝 Versioning
- Changes are tracked in [`CHANGELOG.md`](../CHANGELOG.md).  
- Case IDs follow the rules in [`CASEID_POLICY.md`](../CASEID_POLICY.md).  
- Milestones and upcoming plans are documented in [`ROADMAP.md`](../ROADMAP.md).  

---

## 8. 🤝 Community Contributions
Contributors are encouraged to:
- Suggest new use cases with [issue templates](../.github/ISSUE_TEMPLATE/)  
- Flag incomplete or incorrect entries  
- Propose new taxonomy refinements  
- Share vendor or industry sources not yet covered  

---

## 9. 🎯 Guiding Principles
- **Transparency**: document sources and decisions  
- **Consistency**: follow schema and taxonomy  
- **Responsibility**: avoid hype, focus on *actual AI implementations*  
- **Openness**: encourage collaboration and sharing under MIT License  

---

*This methodology will evolve as the project scales. Feedback and improvements are welcome.*

---
<br>

> ➡️ Back to main [README](../README.md)