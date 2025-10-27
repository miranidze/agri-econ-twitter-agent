
# 🌾 Agricultural Economics Twitter Agent

An automated Python agent that searches Twitter (X) daily for the top 5 most engaging tweets about agricultural economics, filters for verified institutional sources, and delivers a daily summary report via Telegram. 

# 🧭 Overview

This agent automatically:

1. Searches Twitter each day for fresh tweets about agricultural economics, agriculture policy, farm economics, and food supply.

2. Collects only tweets from verified accounts — news agencies, research institutions, companies, or organizations.

3. Ensures no repetition by tracking previously sent tweets.

4. Sends a daily digest containing the top 5 tweets via telegram bot.


# 🗂️ Project Structure (initial)

```
agri-econ-twitter-agent/
├── README.md
├── .env.example
├── requirements.txt
├── main.py
├── search_tweets.py
├── storage.py
├── notify.py
├── utils.py
├── templates/
│   └── daily_digest.html
├── data/
│   └── tweets.db            # runtime
└── .github/
    └── workflows/
        └── daily-run.yml

```

# ⚙️ Features

✅ Automated daily run (via GitHub Actions)

🔍 Smart Twitter search using X API v2

🔐 Environment-based configuration for API keys

🧠 Optional: easily extendable to include AI summaries or policy insights

💾 Local storage of previously sent tweet IDs (JSON or SQLite)

🪶 Lightweight, modular Python design