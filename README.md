<div align="center">

# 🏃 Aerofit: Who Buys Which Treadmill?

**An exploratory data analysis of 180 treadmill buyers that turns customer profiles into a targeting strategy for three products.**

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kartikeyajay2006/Math-EDA/blob/main/Aerofit_case_study.ipynb)
[![pandas](https://img.shields.io/badge/pandas-EDA-150458?style=flat-square&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-visuals-4C72B0?style=flat-square)](https://seaborn.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-notebook-F37626?style=flat-square&logo=jupyter&logoColor=white)](Aerofit_case_study.ipynb)

</div>

---

## The business question

Aerofit sells three treadmills: the entry-level **KP281**, the mid-range **KP481** and the premium **KP781**.
**Which kind of customer buys which model, and how should each one be marketed?**

## Dataset

**180 customers × 9 attributes**: product, age, gender, education, marital status, planned weekly usage, self-rated fitness (1–5), income and expected weekly miles.
There are 104 male and 76 female customers, 107 partnered and 73 single.

## What the analysis covers

1. **Data quality**: shape, types, missing values and duplicates
2. **Feature engineering**: binary `is_married` and `is_male` flags, and income bins
3. **Univariate analysis**: histograms with KDE, count plots and distribution plots for age, education, usage, fitness and miles
4. **Bivariate analysis**: income by gender and by marital status (box plots), and gender against marital status
5. **Multivariate analysis**: correlation heat-map, pair plot, and product mix across income bins
6. **Customer profile per product**: median attributes for each treadmill

## Key findings

| Median | KP281 | KP481 | KP781 |
|---|---|---|---|
| Age | 26 | 26 | 27 |
| Education (years) | 16 | 16 | **18** |
| Usage (days / week) | 3 | 3 | **5** |
| Fitness (1–5) | 3 | 3 | **5** |
| Income ($) | 46,617 | 49,460 | **76,569** |
| Miles / week | 85 | 85 | **160** |

- The **KP281 sells the most**, followed by the KP481. The KP781 sells the least, but its buyers are clearly different.
- KP781 buyers earn about **64% more** than KP281 buyers, run **nearly 2×** the miles and plan to use the treadmill **5 days a week instead of 3**.
- **Fitness, usage, miles and income move together.** Fitter, higher-earning and more committed customers choose the premium model.

## Recommendations

- **KP781: sell performance, not price.** Target customers who already train seriously, with in-store demos of its advanced features.
- **KP281 and KP481: sell simplicity and health.** Use offers, EMIs and bundles to bring in beginners.
- **Help buyers choose** with a short quiz that matches fitness goals and planned usage to a model.
- **Build an upgrade path** from KP281 to KP781, with accessory bundles to raise lifetime value.

## Run it

Click **Open in Colab** above, or run it locally:

```bash
pip install numpy pandas matplotlib seaborn jupyter
jupyter notebook Aerofit_case_study.ipynb
```

The dataset is downloaded automatically from its public URL.

## Author

**[Kartikeya Yadav](https://github.com/kartikeyajay2006)** · [LinkedIn](https://www.linkedin.com/in/kartikeya2006/)
