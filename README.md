# Social Web

**Hands-on assignments for The Social Web: collecting, processing, and analyzing Mastodon data using Python and Jupyter notebooks.**

## Overview

Social Web is a Jupyter-based exploration of social web data using Mastodon. It introduces API-based data collection, text processing, frequency analysis, user engagement analysis, and visualization. The repository starts with the *Social Web — Hands-on Session 1* assignment notebook.

## What you'll explore

1. **Mastodon API** — connect to an instance, inspect server information, retrieve trends and search posts.
2. **Text processing** — clean HTML and extract words, usernames, and hashtags.
3. **Frequency analysis** — compare word and hashtag distributions across queries.
4. **Language statistics** — calculate lexical diversity and average post length.
5. **Engagement** — explore boosts and replies for selected accounts and posts.
6. **Visualization** — create rank-frequency charts and histograms with Matplotlib and Seaborn.

## Quick start

```bash
git clone https://github.com/safouanb/social-web.git
cd social-web
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook notebooks/01_mastodon_exploration.ipynb
```

Create a Mastodon account and obtain API application credentials through your instance's developer settings. The supplied notebook still contains placeholder values: replace them **locally** before running the API exercises. Never commit real keys or access tokens. An `.env.example` is included for a future environment-variable-based setup; the original notebook does not load `.env` automatically.

> **Version note:** The course handout specifies Python 3.8; the notebook itself checks for Python 3.6+ and its saved metadata indicates Python 3.9.6. Python 3.8 is the original course recommendation, not a verified requirement for current dependency releases.

## Repository structure

```text
social-web/
├── notebooks/
│   └── 01_mastodon_exploration.ipynb  # Original session 1 notebook (unfinished exercises)
├── docs/
│   └── getting-started.pdf            # Provided course setup guide
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

## Assignment status

The starter notebook contains six exercises and their original `#Your Code` placeholders. This repo is a **starter**, not a completed assignment. API calls require working credentials and access to a live Mastodon instance; the sample queries and status IDs may need updating.

## Attribution

Course material: *The Social Web*, hands-on session 1 (2026), by the course teaching team listed in the notebook. The accompanying getting-started guide is credited to Michael Accetto, Caio Lopes da Silva, and Jacco van Ossenbruggen (2021). Uploaded teaching material is included for personal coursework; check course redistribution permissions before publishing this repository publicly.
