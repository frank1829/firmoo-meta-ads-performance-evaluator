# Firmoo Meta Ads Performance Evaluator

This repository contains a fully operational scoring and decision-making system for evaluating Meta Ads performance for Firmoo’s Spain market.  
It includes two Jupyter Notebooks:

- **Campaign_decision.ipynb** — evaluates performance at the *campaign level*
- **Ad_decision.ipynb** — evaluates performance at the *ad/creative level*

The goal of this project is to provide a consistent, automated, and data-driven way to identify:
- Which campaigns deserve increased budget  
- Which ads should continue running  
- Which ads should remain in testing  
- Which ads should be paused or redesigned

This system helps reduce subjective judgment, increase evaluation speed, and improve overall advertising ROI.

---

## Features

### 1. Automated Scoring Model  
Each ad or campaign receives a **0–1 performance score** based on the following factors:
- ROAS (Return on Ad Spend)
- CPA & CPM
- Purchase count & spend size (data stability)
- Meta ranking signals (Quality / Engagement / Conversion Ranking)
- Frequency fatigue penalty
- Under-spending protection (avoid misjudging new ads)

### 2. Business-aligned Decision Rules  
The notebooks output clear decision labels, such as:
- **Highly recommended to increase budget**
- **Keep running & optimize**
- **Continue small-scale testing**
- **Insufficient data**
- **Pause or redesign**

All decisions are sorted by business priority.

### 3. Weekly Workflow Ready  
The workflow is designed so that the user can:
1. Export → Meta Ads CSV  
2. Replace the file path in the notebook  
3. Run all cells  
4. Instantly obtain a fully sorted decision table

---

## Repository Structure

