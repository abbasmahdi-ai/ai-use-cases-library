# 📑 Schema – AI Use Cases Library

This file defines the schema for `data/use-cases.csv`  
It ensures **consistency**, **quality**, and **clarity** across all entries.

---

## Columns & Definitions

| Column              | Description                                                                                   | Example |
|---------------------|-----------------------------------------------------------------------------------------------|---------|
| **CaseID**          | Unique identifier for the use case. Format: `aicase-00001` (final), `aicase-x0001` (excluded), `aicase-02261`+ (in-review). See [`CASEID_POLICY.md`](../CASEID_POLICY.md). | `aicase-01542` |
| **Organization**    | Name of the company, institution, or entity implementing AI.                                  | `Siemens Energy` |
| **Use Case Title**  | Concise, descriptive title (not marketing language).                                           | `AI-powered inspection with NVIDIA Triton` |
| **Description**     | Short summary of the problem, solution, and outcome.                                           | `Siemens used NVIDIA Triton for computer vision to automate safety inspections.` |
| **Org Industry**    | The industry of the organization (not vendor). Must match values in [`docs/taxonomy.md`](../docs/taxonomy.md). | `Energy & Utilities` |
| **Use Case Industry** | The primary industry impacted by the use case (can differ from Org Industry if cross-sector). | `Manufacturing` |
| **Subindustry Tags** | Optional tags to refine the industry (comma-separated).                                        | `Hospitals, MedTech` |
| **Use Case Domain** | The functional domain where AI is applied. Must match [`docs/taxonomy.md`](../docs/taxonomy.md). | `Operations & Supply Chain` |
| **Tools/Technologies** | AI models, APIs, platforms, frameworks, or infrastructure used.                             | `NVIDIA Triton Inference Server, TensorFlow` |
| **Outcomes & Benefits** | Tangible results or advantages. Multiple allowed, separated by `;`.                         | `Cost Reduction; Efficiency & Productivity` |
| **Source URL**      | Direct link to the original case study / reference.                                            | `https://www.nvidia.com/en-us/customer-stories/siemens-energy-simplifies-safety-inspections/` |

---

## Formatting Rules
- **Consistency**: Use sentence case for titles and descriptions.  
- **No hype**: Avoid marketing language like “revolutionary” or “cutting-edge.”  
- **Standard taxonomy**: Use industries/domains/outcomes from [`docs/taxonomy.md`](../docs/taxonomy.md).  
- **Multiple values**: Separate by commas (for tags) or semicolons (for outcomes).  
- **URLs**: Must be valid and publicly accessible.  

---

## File Variants
- `data/use-cases.csv` → Final curated cases (v1.0 and beyond).  
- `in-review/use-cases-in-review.csv` → Pending review/normalization.  
- `excluded/use-cases-excluded.csv` → Removed cases (not AI, duplicates, vague).  

---

## Notes
- Each case should be **self-contained** (no missing critical fields).  
- If a source is unavailable (404), move the case to **excluded**.  
- If metadata is incomplete but promising, move it to **in-review**.  

---

*This schema will evolve as new metadata fields (e.g., risk, ethics) are introduced.*

---
<br>

> ➡️ Back to main [README](../README.md)