# CaseID Policy

## Purpose
This document defines the policy for assigning and managing unique CaseIDs across all datasets in the **AI Use Cases Library**.  
CaseIDs ensure that every case ever considered, whether included, in-review, or excluded, remains permanently traceable.  

---

## Format
- **Prefix:** `aicase`  
- **Numbering:** 5-digit zero-padded numbers (e.g., `aicase-00001`)  
- **Separator:** Dash (`-`)  
- **Status-specific prefixes:**  
  - Standard format: `aicase-00001` → `aicase-99999` (used for Final and In-Review)
  - Excluded format: `aicase-x0001` → `aicase-x9999` (traditional excluded cases)  

---

## Numbering Scheme (v2.0)

### Current Ranges
- **Final curated dataset**  
  - CaseIDs: `aicase-00001` → `aicase-03132` (3,023 cases)  
  
- **In-Review dataset**  
  - Various CaseIDs (non-sequential after quality reviews)
  - 78 cases pending validation
  
- **Excluded dataset**  
  - Traditional excluded: `aicase-x0001` → `aicase-x0690` (690 original excluded cases)
  - Migrated from in-review: Various `aicase-#####` IDs (30 cases moved during v2.0 quality review)
  - Total: 720 excluded cases

---

## Status
Each case has a permanent CaseID, but its **status** may change over time.  
- `Final` → Included in the curated dataset (`/data/use-cases.csv`)  
- `In-Review` → Pending review, enrichment/normalization (`/in-review/use-cases-in-review.csv`)  
- `Excluded` → Removed for reasons such as duplication, not truly AI, or insufficient documentation (`/excluded/use-cases-excluded.csv`)  

---

## Permanence
- **CaseIDs are immutable.** Once assigned, a CaseID never changes and is never reused, even if the case is excluded.  
- **Auditability:** The CaseID provides a permanent reference, allowing cases to be tracked across versions and statuses.  
- **Format preservation:** Cases retain their original CaseID format regardless of status changes.

---

## CaseID Format Rules

### Traditional Workflow (Original Cases)
Cases initially identified as likely exclusions receive the `aicase-x####` format:
- Example: `aicase-x0042` → Analytics dashboard mislabeled as AI
- These cases start in `/excluded/` and remain there
- If later deemed valid, they retain `aicase-x####` format even when moved to `In-Review` or `Final`

### In-Review Workflow (Quality Review Process)
Cases initially added to in-review receive standard `aicase-#####` format:
- Example: `aicase-02435` → Startup exploring Claude for summarization
- If later determined to be invalid during quality review, they are moved to `/excluded/`
- **Critical**: They **retain their original non-x CaseID format** (e.g., `aicase-02435`)
- This creates a mixed format in the excluded dataset

### Result
The `/excluded/` dataset contains two CaseID format types:
1. **Traditional format**: `aicase-x0001` → `aicase-x0690` (originally identified as exclusions)
2. **Standard format**: `aicase-#####` (migrated from in-review after quality assessment)

---

## Status Change Examples

### Example 1: Standard In-Review → Final
- **Initial**: `aicase-02350` assigned to in-review case
- **After enrichment**: Case validated and moved to final dataset
- **CaseID**: Remains `aicase-02350`
- **Result**: Case appears in `/data/use-cases.csv` with `aicase-02350`

### Example 2: In-Review → Excluded (New in v2.0)
- **Initial**: `aicase-02435` assigned to in-review case
- **After quality review**: Case determined to be duplicate or non-AI
- **CaseID**: Remains `aicase-02435` (does NOT change to `aicase-x####`)
- **Result**: Case appears in `/excluded/use-cases-excluded.csv` with `aicase-02435`
- **Rationale**: Preserves complete audit trail of quality review process

### Example 3: Traditional Excluded Case
- **Initial**: `aicase-x0042` assigned upon identification as non-AI
- **Status**: Remains in `/excluded/use-cases-excluded.csv`
- **CaseID**: Remains `aicase-x0042`

### Example 4: Excluded → In-Review (Rare)
- **Initial**: `aicase-x0042` in excluded dataset
- **After review**: Case deemed valid after obtaining missing information
- **CaseID**: Remains `aicase-x0042` (does NOT change to standard format)
- **Result**: Case appears in `/in-review/` with `aicase-x0042`
- **If later finalized**: Case appears in `/data/` with `aicase-x0042`

---

## Handling Changes to Published Cases

### Moving from Final to Excluded
Once published in the curated dataset, a case remains permanent unless a **material error** is identified:
- If clearly invalid (duplicate, not AI, broken source): Moved directly to `/excluded/`, retaining original CaseID
- If validity uncertain: May be moved temporarily to `/in-review/` for reassessment
- **CaseID never changes**, only the status is updated

### Example of Final → Excluded
- **Original**: `aicase-01234` published in v1.0 final dataset
- **Discovery**: Case determined to be duplicate of `aicase-00567`
- **Action**: `aicase-01234` moved to `/excluded/use-cases-excluded.csv`
- **CaseID**: Remains `aicase-01234` (standard format, not changed to `aicase-x####`)

---

## Current CaseID Distribution (v2.0)

### Final Dataset (`/data/use-cases.csv`)
- **Count**: 3,023 cases
- **Format**: `aicase-00001` → `aicase-03132` (some numbers skipped due to exclusions)
- **Notes**: Sequential but with gaps where cases were excluded or remain in-review

### In-Review Dataset (`/in-review/use-cases-in-review.csv`)
- **Count**: 78 cases
- **Format**: Various `aicase-#####` IDs (non-sequential)
- **Notes**: Numbers are not consecutive due to cases moving between statuses

### Excluded Dataset (`/excluded/use-cases-excluded.csv`)
- **Count**: 720 cases total
  - ~690 traditional excluded (`aicase-x0001` → `aicase-x0690`)
  - ~30 migrated from in-review (various `aicase-#####` IDs)
- **Format**: Mixed — both `aicase-x####` and `aicase-#####`
- **Notes**: The presence of non-x format IDs indicates cases that were initially considered valid but later excluded

---

## Why CaseID Permanence Matters

### Audit Trail
CaseID permanence creates a complete record:
- `aicase-02435` moving from In-Review → Excluded shows quality review happened
- `aicase-x0042` moving from Excluded → Final shows reassessment occurred
- Format itself tells the story of the case's journey

### Research Integrity
Researchers citing cases can:
- Track a case across versions
- Understand why a case was excluded
- Verify the validation process

### Transparency
The mixed formats in `/excluded/` demonstrate:
- Rigorous quality control (30 in-review cases moved to excluded in v2.0)
- Honest assessment (not all submitted cases meet criteria)
- Continuous improvement (willing to exclude previously accepted cases)

---

## Future Considerations

### Scaling Beyond 99,999 Cases
If the dataset grows beyond `aicase-99999`:
- Transition to 6-digit format: `aicase-100000`
- All existing CaseIDs remain unchanged
- Format rules remain consistent

### Format Changes
Any future changes to CaseID format will:
- Only apply to newly assigned cases
- Never modify existing CaseIDs
- Be documented in this policy

---

## Summary

**Key Principles:**
1. ✅ CaseIDs are **permanent and immutable**
2. ✅ CaseIDs **never change** regardless of status transitions
3. ✅ Format preservation: `aicase-x####` stays `aicase-x####`, `aicase-#####` stays `aicase-#####`
4. ✅ The `/excluded/` dataset may contain **mixed formats** (both `aicase-x####` and `aicase-#####`)
5. ✅ CaseID format tells the story: `x` prefix = originally flagged for exclusion, standard format = went through review process

**Status Transitions Preserve CaseID:**
- In-Review (`aicase-#####`) → Final (`aicase-#####`) ✓
- In-Review (`aicase-#####`) → Excluded (`aicase-#####`) ✓ *New in v2.0*
- Excluded (`aicase-x####`) → In-Review (`aicase-x####`) ✓
- Final (`aicase-#####`) → Excluded (`aicase-#####`) ✓

This policy ensures complete traceability and transparency across the entire lifecycle of every case in the AI Use Cases Library.

---

<br>

> ➡️ Back to [README](./README.md)
