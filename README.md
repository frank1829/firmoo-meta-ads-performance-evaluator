# FACE-DECIDE

**Facebook Ads Performance Scoring & Decision Framework**
Automated decision model for budget allocation and performance evaluation in paid media environments.

---

## 1. Introduction

FACE-DECIDE is a reproducible framework designed to evaluate Facebook advertising performance using standardized rules and weighted scoring.
It converts raw ad metrics into decision outputs, helping teams determine whether an ad should be scaled, maintained, tested further, or paused.

The framework is built for real-world weekly campaign reviews and can be adapted to various markets, product categories, or testing environments.

---

## 2. Repository Contents

| File                                              | Description                                          |
| ------------------------------------------------- | ---------------------------------------------------- |
| `Campaign_decision.ipynb`                         | End-to-end decision pipeline with final label output |
| `facebook_ad_performance_scoring.ipynb`           | Core scoring model and threshold configuration       |
| `Firmoo-ES-Ads-Nov-14-2025-Nov-20-2025.csv`       | Sample ad-level dataset                              |
| `Firmoo-ES-Campaigns-Nov-12-2025-Nov-18-2025.csv` | Sample campaign-level dataset                        |

---

## 3. Model Structure

### Core Logic

| Component          | Purpose                                  |
| ------------------ | ---------------------------------------- |
| Data Validation    | Detect unstable or insufficient samples  |
| Weighted Scoring   | ROAS, Spend, Purchases, CPM              |
| Decision Flow      | Rule-based actions for each ad           |
| Prioritized Output | Sorted recommendation list for execution |

### Decision Labels Output

| Label                              | Interpretation                                    |
| ---------------------------------- | ------------------------------------------------- |
| Strongly Recommend Budget Increase | Stable and scalable performance                   |
| Maintain and Optimize              | Reasonable performance with improvement potential |
| Testing Phase – Data Insufficient  | Do not scale; require further observation         |
| Consider Pausing or Reworking      | Low ROI or high cost                              |
| Sample Too Small                   | Minimum statistical strength not met              |

---

## 4. Usage

```bash
git clone https://github.com/<your_github_username>/FACE-DECIDE.git
cd FACE-DECIDE
pip install -r requirements.txt
jupyter notebook
```

---

## 5. Extension Possibilities

* Integration with automated alert systems (Slack / Notion API)
* Cross-market comparison benchmarking
* Material-level AB testing integration
* Predictive layer for expected ROAS or budget efficiency

---

## 6. License

Released under the MIT License. The framework may be reused or adapted for research and application purposes.

