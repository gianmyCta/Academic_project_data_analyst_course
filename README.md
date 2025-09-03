
# Academic Project — Data Analyst Portfolio

[![Python](https://img.shields.io/badge/Python-3.10%2B-informational)]()
[![Status](https://img.shields.io/badge/Reproducible-Yes-brightgreen)]()
[![License](https://img.shields.io/badge/License-Choose-blue)]()

> **EN** · below in **IT** 🇮🇹

A compact, reproducible portfolio of academic Data Analytics projects. It showcases practical skills in **Python**, **SQL**, **Excel**, and **Power BI/Tableau**, with emphasis on clear EDA, modeling baselines, business‑oriented insights, and clean code.

---

## Projects (overview)

| Project | Topic | Stack | Highlights | Notebook |
|---|---|---|---|---|
| Bitcoin Sentiment | NLP / Sentiment | Python, pandas, scikit-learn, NLTK, matplotlib | Clean & tokenize tweets, TF‑IDF + Logistic baseline, report F1 | `notebooks/bitcoin_sentiment.ipynb` |
| Fake News Filter | NLP / Classification | Python, scikit-learn | Pipeline, cross‑val, feature importance/explainability | `notebooks/filtro_fake_news.ipynb` |
| Customer Segmentation | Clustering | pandas, scikit-learn | K‑means, Silhouette, user personas & actions | `notebooks/segmentazione_clienti.ipynb` |
| F1 Analysis | EDA / Viz | pandas, plotly/matplotlib | Race pace & pit strategy insights, storytelling | `notebooks/progetto_analisi_f1.ipynb` |
| Air Disasters Analysis | EDA / Time series | pandas, matplotlib | Long‑term trends, safety insights, seasonality | `notebooks/analisi_disastri_aerei.ipynb` |

> Replace notebook paths if different in your repo, and add/remove rows as needed.

---

## Quickstart

### 1) Clone & create a virtual environment
```bash
git clone https://github.com/<your-user>/Academic_project_data_analyst_course.git
cd Academic_project_data_analyst_course

# macOS/Linux
python3 -m venv .venv && source .venv/bin/activate

# Windows (PowerShell)
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 2) Install dependencies
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 3) (Optional) Setup environment variables
If a project uses API keys (e.g., Twitter), copy `.env.example` to `.env` and fill values:
```bash
cp .env.example .env
# then edit .env
```

### 4) Launch notebooks
```bash
jupyter lab   # or: jupyter notebook
```

---

## Repository structure (suggested)
```
.
├── notebooks/                 # Exploratory notebooks (thin; call functions from /src)
├── src/                       # Reusable code (ETL, features, models, viz)
│   ├── data/etl.py
│   ├── data/preprocess.py
│   ├── models/text.py
│   └── viz/plots.py
├── reports/                   # Exported figures (PNG/HTML) used in README
├── data/                      # (gitignored) raw/processed datasets
├── tests/                     # Minimal unit tests for functions in /src
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Reproducibility & quality

- **Random seeds**: set for model training and splits.
- **Metrics**: report appropriate metrics (F1/AUC for classification, RMSE/MAE for regression, Silhouette for clustering).
- **Style**: auto‑format with `black`, lint with `ruff` (optional `pre-commit`).
- **Tests**: minimal `pytest` for key helpers in `/src` (e.g., text cleaning, feature scaling).
- **Notebooks**: keep them light; move logic to `/src`. Consider executing via CI (papermill) for smoke tests.

---

## Data sources & compliance

- Do not commit raw data; store under `/data` and **gitignore** it.
- Document dataset **source & license** in each project (README cell or notebook header).
- For APIs (e.g., Twitter), store keys in `.env` (never commit secrets).

---

## Results & reports

Include 1–2 “hero” charts per project in `/reports` and embed them here. Example:

- Fake News Filter — **F1 = 0.86**, macro‑average on holdout, pipeline: TF‑IDF + Logistic.
- Customer Segmentation — **k = 4**, **Silhouette = 0.41**, defined personas and next actions.

---

## About me

I’m a Computer & Automation Engineering graduate, pivoting into **Data Analytics**. Comfortable with Python/SQL/BI and with operational experience in aviation and robotics (cobots).
- LinkedIn: https://www.linkedin.com/in/<your-link>
- CV (EN/IT): link here
- Email: your@email

---

## License

Choose a license (e.g., Apache‑2.0, MIT) and add it as `LICENSE` file. Update the badge at the top accordingly.

---

# 🇮🇹 Italiano

Un portfolio **riproducibile** di progetti accademici in **Data Analytics**. Mostra competenze pratiche in **Python**, **SQL**, **Excel** e **Power BI/Tableau**, con focus su EDA chiara, baseline di modellazione, insight utili al business e codice pulito.

## Progetti (panoramica)

| Progetto | Tema | Stack | Punti chiave | Notebook |
|---|---|---|---|---|
| Sentiment Bitcoin | NLP / Sentiment | Python, pandas, scikit-learn, NLTK, matplotlib | Pulizia/tokenizzazione tweet, TF‑IDF + Logistic baseline, F1 | `notebooks/bitcoin_sentiment.ipynb` |
| Filtro Fake News | NLP / Classificazione | Python, scikit-learn | Pipeline, cross‑val, feature importance/explainability | `notebooks/filtro_fake_news.ipynb` |
| Segmentazione Clienti | Clustering | pandas, scikit-learn | K‑means, Silhouette, personas & azioni | `notebooks/segmentazione_clienti.ipynb` |
| Analisi F1 | EDA / Viz | pandas, plotly/matplotlib | Race pace e strategie pit, storytelling | `notebooks/progetto_analisi_f1.ipynb` |
| Analisi Disastri Aerei | EDA / Serie storiche | pandas, matplotlib | Trend storici, insight sicurezza, stagionalità | `notebooks/analisi_disastri_aerei.ipynb` |

## Avvio rapido

1. Clona repo e crea ambiente virtuale (vedi sopra).
2. Installa dipendenze con `pip install -r requirements.txt`.
3. (Opzionale) Copia `.env.example` in `.env` e inserisci eventuali chiavi API.
4. Avvia `jupyter lab` e apri i notebook.

## Struttura, Reproducibilità, Dati, Risultati

Vedi le sezioni in inglese qui sopra per i dettagli su struttura, metriche, qualità, gestione dati e risultati (grafici **hero** in `/reports`).

---


