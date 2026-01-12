# Analysis Scripts

This folder contains example scripts and notebooks for analyzing the **AI Use Cases Library dataset**.

## Included

- **analysis_notebook.ipynb**  
  A starter Jupyter notebook demonstrating how to:
  - Load the dataset (`../../data/use-cases.csv`)
  - Explore industries, domains, and vendors
  - Run a simple outcomes keyword scan
  - Generate quick bar charts

- **requirements.txt**  
  Minimal dependencies (`pandas`, `matplotlib`).

## Usage

1. Create a virtual environment (optional but recommended).
   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/macOS
   venv\Scripts\activate      # Windows
   ```

2. Install requirements:

   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open `analysis_notebook.ipynb` and run the cells.

## Notes

* The notebook is **minimal by design** for v2.0 — just enough to show dataset loading and simple analysis.
* For deeper insights, see `/insights/` and `/charts/`.
* Contributions of new notebooks or scripts are welcome (see [CONTRIBUTING](../../docs/contributing.md)).

