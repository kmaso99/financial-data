# Financial Data Analyses 📈💰📊

A collection of **financial analytics and applied data science case studies** in Jupyter notebooks.

Focus: clean data workflows, feature engineering, model evaluation, and clear business-facing outputs.

---

## Start here (recommended order)

1. **BCGX Task One**
   https://github.com/kmaso99/financial-data/blob/main/BCGX%20Task%20One.ipynb

2. **BCGX Task Two**
   https://github.com/kmaso99/financial-data/blob/main/BCGX%20Task%20Two.ipynb

3. **BCGX Task Three**
   https://github.com/kmaso99/financial-data/blob/main/BCGX%20Task%20Three.ipynb

4. **BCGX Task Four**
   https://github.com/kmaso99/financial-data/blob/main/BCGX%20Task%20Four.ipynb

5. **Quantium Part I**
   https://github.com/kmaso99/financial-data/blob/main/Quantium%20Part%20I.ipynb

6. **Quantium Part II**
   (link in repo if present; if Part II is only a checkpoint file, consider committing the non-checkpoint version)

---

## What these notebooks demonstrate

This repo emphasizes the practical skills hiring managers look for in finance/analytics work:

- Data cleaning and tidy dataset construction
- Feature engineering for structured/tabular problems
- Baselines, model selection, and evaluation discipline
- Interpretable outputs (plots, diagnostics, and concise takeaways)

---

## Notes on reproducibility

These notebooks are designed to be readable first, reproducible second:
- assumptions and transformations are documented inline
- random seeds are set when modeling is involved
- outputs are generated from code (not manually edited)

If you want to run locally, the typical setup is:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
