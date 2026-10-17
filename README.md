<p align="center">
  <img src="https://raw.githubusercontent.com/VibhoreKumar/VibhoreKumar/b4568e187095325597bbd4e77521bb094a9f455d/assets/01-cover.svg" width="100%" alt="VK — Vibhore Kumar, aspiring data engineer. Python, SQL, ETL, APIs and analytics." />
</p>

<p align="center">
  <a href="https://linkedin.com/in/vibhore-kumar-9b9298376"><img src="https://img.shields.io/badge/LINKEDIN-126568?style=flat-square" alt="LinkedIn" /></a>
  <a href="mailto:vibhore098sharma@gmail.com"><img src="https://img.shields.io/badge/EMAIL-126568?style=flat-square" alt="Email Vibhore" /></a>
  <a href="https://github.com/VibhoreKumar?tab=repositories"><img src="https://img.shields.io/badge/EXPLORE_MY_WORK-171D1E?style=flat-square" alt="Explore my repositories" /></a>
</p>

I'm **Vibhore Kumar**, a **B.Tech CSE student at GD Goenka University (2027)**, building towards a career in **data engineering**. I work with Python, SQL and APIs to collect, transform and explore data. My full-stack experience helps me connect pipelines to applications people can actually use.

<p align="center">
  <a href="#data-projects">Data projects</a> ·
  <a href="#skills-by-purpose">Skills</a> ·
  <a href="#currently-learning">Learning</a> ·
  <a href="#contribution-heatmap">Activity</a>
</p>

<br />

<img src="https://raw.githubusercontent.com/VibhoreKumar/VibhoreKumar/b4568e187095325597bbd4e77521bb094a9f455d/assets/02-field-notes.svg" width="100%" alt="Data workflow: ingest APIs and files; transform with Python and SQL; store in PostgreSQL or JSON Lines; serve dashboards and analysis. Learning PySpark, Databricks and Delta Lake." />

## Data projects

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

## Currently learning

**PySpark · Databricks · Delta Lake**

My next focus is moving from small Python pipelines towards distributed data processing: practising DataFrame transformations, exploring lakehouse storage and connecting processed datasets to dashboards.

## Experience behind the pipelines

- **WebArclight · Full-Stack Developer Intern · Oct 2025–Jan 2026** — worked with React, Django and REST APIs on application features and integrations.
- **UptoSkills · Web Development Intern · Jul–Sep 2025** — contributed to web development using the MERN stack.

These experiences shaped how I approach API integration, application requirements and delivering usable outputs.

<details>
<summary><b>More about me</b></summary>

- Built web projects including a team AI Resume Builder.
- U-19 state cricket experience, representing Kota, Rajasthan.
- Python Essentials certification.
- Practising DSA: [LeetCode](https://leetcode.com/u/8ZHi5hqRLR) · [GeeksforGeeks](https://geeksforgeeks.org/profile/vibhore092k0l).

</details>

## Contribution heatmap

<p align="center">
  <a href="https://github.com/VibhoreKumar?tab=overview">
    <img src="https://ghchart.rshah.org/126568/VibhoreKumar" width="100%" alt="Vibhore Kumar's GitHub contribution heatmap over the past year" />
  </a>
</p>

## Community badges

<p align="center">
  <a href="https://www.holopin.io/@vibhorekumar">
    <img src="https://holopin.io/api/user/board?user=vibhorekumar&amp;refresh=20261013T002449" width="100%" alt="Vibhore Kumar’s Holopin badge board" />
  </a>
</p>

---

<p align="center"><b>Let's build something that makes data useful.</b><br />Open to data engineering internships, entry-level opportunities and collaboration.</p>

<p align="center">
  <a href="mailto:vibhore098sharma@gmail.com"><img src="https://img.shields.io/badge/GET_IN_TOUCH-126568?style=for-the-badge" alt="Get in touch by email" /></a>
  <a href="https://linkedin.com/in/vibhore-kumar-9b9298376"><img src="https://img.shields.io/badge/CONNECT_ON_LINKEDIN-171D1E?style=for-the-badge" alt="Connect on LinkedIn" /></a>
</p>

<p align="center"><sub>Learning in public · Building one pipeline at a time · India</sub></p>
