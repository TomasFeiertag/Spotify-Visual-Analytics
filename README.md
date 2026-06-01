<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:1DB954,100:0d1117&height=180&section=header&text=Spotify%20Visual%20Analytics&fontSize=40&fontColor=ffffff&animation=twinkling&fontAlignY=38&desc=Interactive%20Power%20BI%20Dashboard%20%7C%20Spotify%20API%20%2B%20Kaggle&descAlignY=60&descSize=18&descColor=a8f0c6" />

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Spotify](https://img.shields.io/badge/Spotify%20API-1DB954?style=for-the-badge&logo=spotify&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)

</div>

---

## 📌 Overview

End-to-end data project combining **Spotify API** live data with the *Most Streamed Spotify Songs 2024* Kaggle dataset to build a fully interactive Power BI dashboard with deep insights into music trends, artist performance, and streaming behavior.

---

## 📊 Dashboard Preview

![Spotify Dashboard](images/Dashboard.jpeg)

---

## 🚀 Features

| Feature | Description |
|---|---|
| 🎵 **Track Explorer** | Filter by date, artist, track, and year |
| 📊 **Stream Analytics** | Distribution charts, timeline of releases, streaming counts |
| 🖼️ **Album Art** | Fetched live from Spotify API |
| 📋 **Playlist Reach** | Metrics on playlist appearances and audience reach |
| 📈 **Rank & Averages** | Track ranking and average streams per year |
| 🔄 **Reset Filters** | One-click dashboard reset |

---

## 🔄 Pipeline

```
Spotify API ──┐
              ├──► ETL (Python + Pandas) ──► Cleaned CSV ──► Power BI Dashboard
Kaggle CSV ───┘
```

**ETL Steps:**
- Authenticated requests to Spotify API using `client_id` / `client_secret`
- Searched each track by artist to retrieve `track_id` and album artwork URLs
- Merged with Kaggle streaming metrics dataset
- Handled nulls, duplicates, and type conversions
- Exported `updated_file.csv` ready for Power BI

---

## ⚒️ Tech Stack

| Layer | Tools |
|---|---|
| **Data Extraction** | Spotify API, Kaggle |
| **Processing** | Python, Pandas |
| **Visualization** | Power BI |

---

## ▶️ How to Run

**1. Clone the repo**
```bash
git clone https://github.com/TomasFeiertag/Spotify-Visual-Analytics.git
cd Spotify-Visual-Analytics
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Set your Spotify API credentials**
```python
client_id = "your_client_id"
client_secret = "your_client_secret"
```

**4. Run the ETL script**
```bash
python scripts/spotify_data_extraction.py
```

**5. Open `spotify_dashboard.pbix` in Power BI Desktop**

---

## 👤 Author

**Tomás Feiertag** — Data Scientist · NLP & LLMs @ Movistar

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/tfeiertag/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/TomasFeiertag)

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1DB954&height=100&section=footer" />
