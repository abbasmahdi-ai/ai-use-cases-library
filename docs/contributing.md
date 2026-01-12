# Contributing to AI Use Cases Library

Thank you for your interest in contributing! 
This project thrives on community input — from suggesting new use cases to refining taxonomy, fixing errors, or improving documentation.

---

## Contribution Workflow

1. **Fork the repository**  
Click the **Fork** button at the top right of this repo to create your own copy.

2. **Clone your fork locally**  
   ```bash
   git clone https://github.com/abbasmahdi-ai/ai-use-cases-library.git
   cd ai-use-cases-library
   ```

3. **Create a feature branch**
   ```bash
   git checkout -b add-new-use-case
   ```

4. **Make your changes**
- Add or edit use cases in [data/] or [in-review/]
- Update [docs], [methodology], or [taxonomy] if needed

  Run notebooks in [tools/analysis-scripts/] if adding analyses

5. **Commit your changes**
   ```bash
   git add .
   git commit -m "Add: [short description of change]"
   ```

6. **Push your branch**
   ```bash
   git push origin add-new-use-case
   ```

7. **Open a Pull Request (PR)**
Go to your fork on GitHub and click Compare & pull request.
Please describe what you changed and link to relevant issue templates.

---

## Use Case Guidelines

- Format: Follow the schema in [data/schema.md](data/schema.md).
- Accuracy: Only include verified AI implementations (not just "AI-powered" marketing).
- Completeness: Include industry, domain, tools/technologies, and clear outcomes.
- Clarity: Write short, descriptive titles and concise summaries.

---

## Issues & Templates

- [New Use Case](../.github/ISSUE_TEMPLATE/new-use-case.yaml)
- [Correction / Update](../.github/ISSUE_TEMPLATE/correction.yaml)

Please use these templates so submissions remain consistent.

---

## Style Notes

- Use sentence case for titles.
- Keep descriptions concise but specific.
- Use American English spelling (e.g., “organization” not “organisation”).
- Avoid vendor hype — focus on the actual AI applied.

---

## License

By contributing, you agree that your contributions will be licensed under the [MIT License](../LICENSE).

---

💡 Tip: If unsure about where a use case fits, open a draft issue first for discussion before submitting a PR.

---
<br>

> ➡️ Back to main [README](../README.md)