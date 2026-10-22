<!-- Pixel-world design adapted from the supplied reference. Commit-pinned artwork avoids stale image caches. -->
<p align="center">
<a href="#selected-builds"><img src="https://raw.githubusercontent.com/VibhoreKumar/VibhoreKumar/717d030efef702a5bfe0f84653da8af871527569/assets/01-cover.svg" width="100%" alt="Vibhore Kumar's pixel world. Press start to explore projects. Aspiring data engineer, B.Tech CSE at GD Goenka University, class of 2027. Python, SQL, PostgreSQL, ETL, APIs and Streamlit. Learning PySpark, Databricks and Delta Lake." /></a>
</p>

<p align="center">
<a href="#selected-builds">▶ PRESS START</a> ·
<a href="#skills-by-purpose">MY STACK</a> ·
<a href="https://linkedin.com/in/vibhore-kumar-9b9298376">LINKEDIN</a> ·
<a href="mailto:vibhore098sharma@gmail.com">CONTACT</a>
</p>

## Selected builds

| LEVEL 01 / DealSense | LEVEL 02 / Weather ETL |
| --- | --- |
| **Creator data → useful insights.** YouTube API ingestion, Python transformations, PostgreSQL storage and a Streamlit dashboard. | **Live weather → historical records.** Open-Meteo ingestion, temperature classification, JSON Lines storage and read-only analysis. |
| Python · SQL · Supabase · Streamlit | Python · REST API · JSON Lines |
| [Explore code →](https://github.com/VibhoreKumar/youtube-creator-analytics) · [Play demo →](https://youtube-creator-analytics-jflipbqujlpcp4xnvmmuaa.streamlit.app/) | [Explore code →](https://github.com/VibhoreKumar/mini_weather_ETL_pipeline) |

<sub>DealSense uses real creator metrics with clearly labelled modeled campaign costs. Engagement anomalies are statistical flags, not proof of fraud.</sub>

<details>
<summary><b>Inside the projects — architecture, stack &amp; data sources</b></summary>

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


</details>

<details>
<summary><b>My toolkit — skills by purpose</b></summary>

## Skills by purpose

| Area | Tools & hands-on work |
| --- | --- |
| **Ingestion** | Python, REST APIs, JSON, nested API responses |
| **Transformation** | Python cleaning and classification, SQL, creator tiering and engagement analysis |
| **Storage** | PostgreSQL / Supabase, JSON Lines; SQLite and MySQL familiarity |
| **Analytics & delivery** | Streamlit dashboards, SQL querying, API-backed applications |
| **Development workflow** | Git, GitHub, GitHub Actions, Postman |
| **Supporting application skills** | React, Django REST Framework, Node.js, Express, MongoDB |


</details>

<details>
<summary><b>My background — experience &amp; beyond code</b></summary>

## Experience behind the pipelines

- **WebArclight · Full-Stack Developer Intern · Oct 2025–Jan 2026** — worked with React, Django and REST APIs on application features and integrations.
- **UptoSkills · Web Development Intern · Jul–Sep 2025** — contributed to web development using the MERN stack.

These experiences shaped how I approach API integration, application requirements and delivering usable outputs.

### Beyond code

- Built web projects including a team AI Resume Builder.
- U-19 state cricket experience, representing Kota, Rajasthan.
- Python Essentials certification.
- Practising DSA: [LeetCode](https://leetcode.com/u/8ZHi5hqRLR) · [GeeksforGeeks](https://geeksforgeeks.org/profile/vibhore092k0l).




</details>

<br />

<img src="https://raw.githubusercontent.com/VibhoreKumar/VibhoreKumar/717d030efef702a5bfe0f84653da8af871527569/assets/02-field-notes.svg" width="100%" alt="Save points — contribution activity" />

<p align="center">
<a href="https://github.com/VibhoreKumar?tab=overview"><img src="https://ghchart.rshah.org/F244A4/VibhoreKumar" width="100%" alt="Vibhore Kumar's GitHub contribution heatmap over the past year" /></a>
</p>

<br />

<img src="https://raw.githubusercontent.com/VibhoreKumar/VibhoreKumar/717d030efef702a5bfe0f84653da8af871527569/assets/03-projects.svg" width="100%" alt="Collectibles — Holopin badge collection" />

<p align="center">
<a href="https://www.holopin.io/@vibhorekumar"><img src="https://holopin.io/api/user/board?user=vibhorekumar&amp;refresh=20261013T002449" width="100%" alt="Vibhore Kumar's Holopin badge board" /></a>
</p>

---

<p align="center"><b>NEXT QUEST: BUILD SOMETHING USEFUL.</b><br /><sub>Open to data engineering internships, entry-level roles and collaboration.</sub></p>
<p align="center"><a href="mailto:vibhore098sharma@gmail.com">[ SEND A MESSAGE ]</a> · <a href="https://github.com/VibhoreKumar?tab=repositories">[ EXPLORE MY WORLD ]</a></p>
