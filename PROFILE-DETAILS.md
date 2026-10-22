# Vibhore Kumar — projects, skills and experience




### 01 / DealSense — Creator ROI Intelligence

**From YouTube API data to a decision-support dashboard.**

A pipeline and dashboard for exploring creators, comparing engagement and planning sponsorship budgets.

| Stage | What the project does |
| --- | --- |
| Ingest | Fetches creator and recent-video data from YouTube Data API v3 |
| Transform | Cleans records, assigns creator tiers and flags unusual engagement within category/tier groups |
| Store | Loads processed data into Supabase PostgreSQL |
| Serve | Presents analytics in Streamlit, with Gemini-assisted SQL questions and explanations |

**Stack:** Python · SQL · PostgreSQL · Supabase · Streamlit · YouTube API · Gemini  
**Data transparency:** Creator metrics come from YouTube; campaign costs are a clearly labelled synthetic layer. Anomaly flags indicate unusual patterns, not proof of fraud.

[Explore the pipeline](https://github.com/VibhoreKumar/youtube-creator-analytics) · [Open the dashboard](https://youtube-creator-analytics-jflipbqujlpcp4xnvmmuaa.streamlit.app/) · [Data sources & limitations](https://github.com/VibhoreKumar/youtube-creator-analytics/blob/main/docs/about_the_data.md)

---

### 02 / Weather ETL — API to historical data

**A focused ETL project built with Python's standard library.**

Collects live weather readings from Open-Meteo, extracts fields from nested JSON, classifies temperatures and appends clean records to a historical log.

| Stage | What the project does |
| --- | --- |
| Extract | Requests weather data for configured cities from Open-Meteo |
| Transform | Selects fields and classifies readings as Hot, Cold or Normal |
| Load | Appends records in JSON Lines format |
| Analyze | Computes category breakdowns and average temperature per city with a separate read-only script |

**Stack:** Python · urllib · JSON · REST API · File-based storage  
**Engineering focus:** Separation of extraction, transformation, storage and analysis; preserving history across runs.

[View source & run instructions](https://github.com/VibhoreKumar/mini_weather_ETL_pipeline)







## Skills by purpose

| Area | Tools & hands-on work |
| --- | --- |
| **Ingestion** | Python, REST APIs, JSON, nested API responses |
| **Transformation** | Python cleaning and classification, SQL, creator tiering and engagement analysis |
| **Storage** | PostgreSQL / Supabase, JSON Lines; SQLite and MySQL familiarity |
| **Analytics & delivery** | Streamlit dashboards, SQL querying, API-backed applications |
| **Development workflow** | Git, GitHub, GitHub Actions, Postman |
| **Supporting application skills** | React, Django REST Framework, Node.js, Express, MongoDB |







## Experience behind the pipelines

- **WebArclight · Full-Stack Developer Intern · Oct 2025–Jan 2026** — worked with React, Django and REST APIs on application features and integrations.
- **UptoSkills · Web Development Intern · Jul–Sep 2025** — contributed to web development using the MERN stack.

These experiences shaped how I approach API integration, application requirements and delivering usable outputs.

### Beyond code

- Built web projects including a team AI Resume Builder.
- U-19 state cricket experience, representing Kota, Rajasthan.
- Python Essentials certification.
- Practising DSA: [LeetCode](https://leetcode.com/u/8ZHi5hqRLR) · [GeeksforGeeks](https://geeksforgeeks.org/profile/vibhore092k0l).




