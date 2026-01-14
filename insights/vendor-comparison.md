# Vendor Presence in Documented AI Use Cases

We analyzed 3,023 documented enterprise AI use cases. Vendor presence was measured two ways:  

1. **Tool/Technology mentions** → where a vendor's products appear in the Tool/Technology column.  
   - Captures multi-vendor adoption.  
   - Shows technical footprint across use cases.  

2. **Source (Publisher)** → who published the case study.  
   - Reflects marketing and publication bias.  
   - Vendors like Microsoft and Google publish far more case studies than others.  

> ℹ️ **Note:** See the [README note on vendor presence](../README.md) for methodology and limitations.  
> These figures represent the *share of documented case studies in our dataset*, not true global adoption. Vendors with larger publication pipelines (e.g., Microsoft, Google) may appear overrepresented.
---

## 🏆 Vendor Presence by Tool/Technology


![Vendor by Tool Mentions](../charts/vendor_by_tools.png)


| Vendor | Tool/Technology Mentions | % of Dataset |
|--------|--------------------------|--------------|
| **Microsoft** | 768 | 25.4% |
| **Google** | 726 | 24.0% |
| **OpenAI** | 500 | 16.5% |
| **AWS** | 370 | 12.2% |
| **NVIDIA** | 239 | 7.9% |
| **IBM** | 221 | 7.3% |
| **Anthropic** | 215 | 7.1% |

**Takeaway:** Microsoft and Google dominate due to Azure + Copilot and Gemini ecosystems, while OpenAI and Anthropic show strong technical presence despite publishing fewer cases directly.

---

## 📰 Vendor Presence by Source (Publisher)

![Vendor by Source Publisher](../charts/vendor_by_source.png)

| Publisher | Published Cases | % of Dataset |
|-----------|-----------------|--------------|
| **Google** | 996 | 32.9% |
| **Microsoft** | 755 | 25.0% |
| **AWS** | 297 | 9.8% |
| **NVIDIA** | 218 | 7.2% |
| **IBM** | 217 | 7.2% |
| **Anthropic** | 175 | 5.8% |
| **OpenAI** | 151 | 5.0% |

**Takeaway:** Google leads in publication volume (33% of all cases), followed by Microsoft. OpenAI and Anthropic publish fewer cases directly, even though their models are widely used through partners.

---

## 🔍 The Multiplier Effect

**OpenAI** appears in 500 tool mentions but only published 151 cases directly. **Why the gap?**

Because Azure OpenAI Service deployments get counted as both "Microsoft" and "OpenAI." Similarly, **Anthropic** appears in 215 tool mentions but published 175 cases directly. The rest come through AWS Bedrock.

**What this means:** The actual usage patterns are murkier than the numbers suggest. A case listed under "Microsoft + OpenAI + Azure" tells you about partnerships and distribution channels, but not necessarily about which technology actually drove the value.

This isn't a flaw in the data. It's a feature of how AI is actually deployed. Multi-vendor solutions are common. But it makes "market share" calculations misleading.

---

## 🔑 Top Tools & Platforms

| Tool/Platform              | Documented Mentions |
|-----------------------------|----------------------|
| Azure OpenAI Service       | 181 |
| Amazon Bedrock             | 160 |
| Microsoft 365 Copilot      | 106 |
| Microsoft Azure            | 103 |
| Anthropic API / Claude     | 101 |
| Vertex AI                  | 90 |
| Amazon SageMaker           | 82 |
| GitHub Copilot             | 53 |
| IBM watsonx Assistant      | 36 |
| Google Gemini              | 30+ |

**Key Observation:** Microsoft owns 93% of the "Copilot" mentions in our dataset.

---

## 🏢 Industry Distribution (by Tool Mentions)

Microsoft, OpenAI, and Anthropic are visible across all major industries. Notable highlights:  
- **Financial Services:** Microsoft (96 cases), AWS and Google present.  
- **Healthcare:** Microsoft Azure dominates (79 cases); OpenAI drives research breakthroughs.  
- **Technology:** Anthropic favored by startups (44 cases).  
- **Retail & E-commerce:** Google Gemini leads in personalization (45 cases).  

---

## 🎯 Takeaways

- **Google** leads in publication volume (33% of cases), showing aggressive content marketing.
- **Microsoft** dominates enterprise presence, both technically (25% of tool mentions) and in published cases (25%).  
- **OpenAI** shows strong technical adoption (17% of tool mentions) despite publishing only 5% of cases directly.
- **Anthropic** appears in 7% of tool mentions, with 175 published cases (6%), showing strong presence for a newer entrant.
- **AWS** offers flexible, multi-model hosting with Bedrock (12% tool mentions).  
- **Google** is strong in retail/e-commerce and has highest publication velocity.
- **IBM** remains in legacy sectors (7% of tool mentions, 7% of publications).  
- **NVIDIA** thrives as AI infrastructure backbone (8% tool mentions, 7% publications).  

---

**Conclusion:**  
This vendor comparison shows not just *who is building AI solutions*, but also *who is publishing them*.  
- Tool mentions reveal **technical adoption**.  
- Source counts reveal **marketing activity**.  

Both perspectives matter – and together they highlight:
- **Google's publication dominance** (996 cases, 33%)
- **Microsoft's enterprise lock-in** (768 tool mentions, 755 publications)
- **OpenAI's deployment-to-publication multiplier** (3.3x: 500 mentions vs 151 publications)
- **Anthropic's rise** in high-value use cases (215 tool mentions, 175 publications)

---
<br>

> ➡️ Back to [README](../README.md)
