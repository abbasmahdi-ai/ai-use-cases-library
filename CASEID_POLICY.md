# CaseID Policy

## Purpose
This document defines the policy for assigning and managing unique CaseIDs across all datasets in the **AI Use Cases Library**.  
CaseIDs ensure that every case ever considered—whether included, in-review, or excluded—remains permanently traceable.  

---

## Format
- **Prefix:** `aicase`  
- **Numbering:** 5-digit zero-padded numbers (e.g., `aicase-00001`)  
- **Separator:** Dash (`-`)  
- **Status-specific ranges:**  
  - Final & In-Review: `aicase-00001` → `aicase-09999`  
  - Excluded: `aicase-x0001` → `aicase-x9999`  

---

## Numbering Scheme
- **Final curated dataset (public v1.0)**  
  - CaseIDs: `aicase-00001` → `aicase-02260` (2,260 cases)  
- **In-Review dataset**  
  - CaseIDs: `aicase-02261` → `aicase-02526` (266 cases)  
- **Excluded dataset**  
  - CaseIDs: `aicase-x0001` → `aicase-x0690` (690 cases)  

---

## Status
Each case has a permanent CaseID, but its **status** may change over time.  
- `Final` → Included in the curated dataset (`/data/use-cases.csv`)  
- `In-Review` → Pending enrichment/normalization (`/in-review/use-cases-in-review.csv`)  
- `Excluded` → Removed for reasons such as duplication, not truly AI, or insufficient documentation (`/excluded/use-cases-excluded.csv`)  

---

## Permanence
- **CaseIDs are immutable.** Once assigned, a CaseID never changes and is never reused, even if the case is excluded.  
- **Auditability:** The CaseID provides a permanent reference, allowing cases to be tracked across versions and statuses.  

---

## Exceptional Situations
In the unlikely case where an excluded case is later reinstated (e.g., due to a categorization mistake or missing information now resolved):  
- The case **retains its original `aicase-x####` ID**.  
- Only its **status changes** (e.g., from `Excluded` → `In-Review` → `Final`).  
- This ensures a complete audit trail while keeping CaseIDs permanent and stable.  

---

## Handling Changes to Published Cases
- Once published in the curated dataset, a case remains permanent unless a **material error** is identified.  
- If the case is clearly invalid (e.g., duplicate, not AI, broken source), it is moved directly to `/excluded/`, retaining its CaseID.  
- In the unlikely case where validity is uncertain, the case may be moved temporarily to `/in-review/` for reassessment.  
- In all cases, the CaseID is never changed or reused; only the `Status` is updated.  

---

## Examples
- **Final case:** `aicase-00123` → “Bank X uses GPT-4o for compliance automation”  
- **In-Review case:** `aicase-02310` → “Startup Y exploring Claude for summarization”  
- **Excluded case:** `aicase-x0042` → “Analytics dashboard mislabeled as AI” (removed for not being true AI)  
- **Reinstated case:** `aicase-x0042` moves from `Excluded` → `In-Review` (retains ID `aicase-x0042`).  

---
<br>

> ➡️ Back to [README](./README.md)