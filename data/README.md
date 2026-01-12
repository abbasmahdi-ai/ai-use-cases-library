# 📂 Data – AI Use Cases Library

This folder contains the **core dataset** of the AI Use Cases Library.  
All use cases follow the structure defined in [`schema.md`](schema.md).

---

## Files

- **`use-cases.csv`**  
  The **final curated dataset**.  
  - 3,023 use cases (as of v2.0)  
  - Cleaned, normalized, and fully tagged using the taxonomy  
  - Only **production-ready** cases are included here

- **`schema.md`**  
  Data dictionary and field definitions.  
  Explains each column and formatting rules.

- **`vendors/`** *(optional)*  
  Contains vendor/model-specific breakdowns (e.g., AWS-only, Microsoft-only).

- **`example.csv`**  
  A **template row** showing correct formatting for new use cases.  
  Contributors should follow this pattern.

---

## Related Folders

- [`../in-review/`](../in-review/)  
  Contains **pending cases** that need more metadata or validation.  
  - These are not yet part of the main dataset.  
  - Moved to `data/use-cases.csv` after review.

- [`../excluded/`](../excluded/)  
  Contains **removed cases** (duplicates, vague, or not truly AI).  
  - Includes a short reason for exclusion.  
  - Helps document what was considered but not included.

---

## Contribution Notes
- Add new use cases to **in-review** first unless they meet all schema requirements.  
- Do **not** edit `use-cases.csv` directly without review.  
- Always validate against the schema in [`schema.md`](schema.md).  

---

✅ For details on contributing, see [`../docs/contributing.md`](../docs/contributing.md).

---
<br>

> ➡️ Back to main [README](../README.md)
