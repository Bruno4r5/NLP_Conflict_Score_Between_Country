# Conflict-Score  
*A weekly, country-pair risk indicator*

## Overview  
This group project builds an automated **Conflict-Score** that tracks week-to-week financial tensions between any two countries. It mines ~33 000 Reuters / CNBC article descriptions (2017-2020) with **spaCy** NER and **FinBERT** sentiment, then weights the signal by bilateral trade flows to amplify economically significant frictions:contentReference[oaicite:0]{index=0}.

## Repository layout
| Notebook | Purpose |
|-----------|---------|
| **01_inspect.ipynb** | Data overview & sanity checks |
| **02_preprocess_and_ner.ipynb** | Cleaning + country-pair extraction |
| **03_sentiment.ipynb** | FinBERT sentiment classification |
| **04_Compute_Score.ipynb** | Score construction & visuals |
| **us_china_conflict_score.ipynb** | U.S.–China case study |

## Quick start
```bash
git clone https://github.com/<your-org>/conflict-score.git
cd conflict-score
pip install -r requirements.txt   # Python ≥3.10
jupyter notebook                  # run notebooks 01→04
