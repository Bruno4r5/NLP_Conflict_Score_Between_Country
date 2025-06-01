# Conflict-Score  
*A weekly, country-pair risk indicator*

## Overview  
This mgroup project tracks week-to-week financial tensions between any two countries. It combines **spaCy** NER and **FinBERT** sentiment on news headlines, then weights the signal by bilateral trade flows to amplify economically significant frictions.

## Data  
| Source | Description |
|--------|-------------|
| **Financial News Headlines**<br>*(Kaggle - Lucas Pham)* | 33 k headlines & previews from **CNBC, The Guardian, Reuters** covering U.S. business news *(Dec 2017 – Jul 2020)*. Used as the raw corpus for NER + sentiment. |

## Repository layout
| Notebook | Purpose |
|-----------|---------|
| **01_inspect.ipynb** | Data overview & sanity checks |
| **02_preprocess_and_ner.ipynb** | Cleaning + country-pair extraction |
| **03_sentiment.ipynb** | FinBERT sentiment classification |
| **04_Compute_Score.ipynb** | Score construction & visuals |
| **us_china_conflict_score.ipynb** | U.S.–China case study |
