# SMNA2026 Assignment 2 — Public Sentiment Toward Electric Vehicles in Australia

## Research Question
> "How has public sentiment toward electric vehicles evolved in Australian Reddit communities,
> and what network structures and topics drive the EV conversation?"

## Team Members
- Ansh Anand Parekh — s4060237
- Disha Dogra — s4091900
- Syna Arora — s4109652

## Course
COSC 3047 — Social Media and Network Analysis
RMIT University — Semester 1, 2026

---

## Project Overview

This project analyses public sentiment toward Electric Vehicles (EVs)
in Australian Reddit communities using Social Media and Network Analysis techniques.

### Key Analysis Components:
1. **Data Collection** — Reddit posts and comments via Arctic Shift (no API key needed)
2. **Preprocessing** — Text cleaning, filtering, keyword matching
3. **Network Analysis** — User interaction graphs, community detection, centrality measures
4. **NLP & Sentiment** — VADER sentiment over time, LDA topic modelling
5. **Discussion** — Trends over time, influential users, key EV concerns

---

## Data Sources

| Subreddit | Focus |
|---|---|
| r/australia | General Australian public opinion on EVs |
| r/ausEV | Dedicated Australian EV community |
| r/AusFinance | EV cost and financial discussions |
| r/electricvehicles | Broader EV discussions (Australian-filtered) |

**Collection method:** Arctic Shift (https://arctic-shift.photon-reddit.com/)
**Date range:** January 2023 — December 2024
**Keywords:** "electric vehicle", "EV", "Tesla", "charging", "battery electric"
**No API key required — Arctic Shift is a free public academic archive**

---

## Project Structure

```
SMNA2026-Assignment2/
│
├── README.md
├── .gitignore
├── requirements.txt
│
├── data/
│   ├── raw/           # Raw collected data from Arctic Shift
│   ├── processed/     # Cleaned and processed data
│   └── sample/        # 10MB sample for submission
│
├── notebooks/
│   ├── 01_data_collection.ipynb      # Collect Reddit EV data
│   ├── 02_data_preprocessing.ipynb   # Clean and prepare data
│   ├── 03_network_analysis.ipynb     # Network graphs and communities
│   ├── 04_nlp_sentiment.ipynb        # Sentiment and topic modelling
│   └── 05_discussion.ipynb           # Final analysis and visualisations
│
├── src/
│   ├── data_collection.py     # Data collection functions
│   ├── network_builder.py     # Network construction functions
│   └── sentiment_analysis.py  # NLP and sentiment functions
│
├── reports/
│   └── figures/       # All visualisations and charts
│
└── worksheets/
    ├── project_plan.pdf
    └── timesheets.pdf
```

---

## Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/Ansh2502/SMNA2026-Assignment2.git
cd SMNA2026-Assignment2
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run notebooks in order
```
01_data_collection.ipynb     
02_data_preprocessing.ipynb
03_network_analysis.ipynb
04_nlp_sentiment.ipynb
05_discussion.ipynb          
```

---

## Ethics & Legal

Data collected from publicly available Reddit posts via Arctic Shift,
a free academic archive compliant with Reddit's Terms of Service.
No private, sensitive or credential data was collected or stored.
Usernames are anonymised in analysis outputs.

---

## References
- Arctic Shift: https://arctic-shift.photon-reddit.com/
- VADER Sentiment: https://github.com/cjhutto/vaderSentiment
- NetworkX: https://networkx.org/
- Gensim LDA: https://radimrehurek.com/gensim/