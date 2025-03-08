# 🎵 Spotify Clusters: A Music Recommendation System 🎧  
*A simple yet effective project that clusters Spotify tracks by audio features to recommend similar songs!*

---

## 📌 Overview  
This project explores clustering techniques on Spotify music tracks (125 genres, 21 audio features) to build a **music recommendation system**. By grouping tracks into clusters and analyzing their features, the system suggests songs that are the closest to your favorites. 

---

## 🗂️ Dataset  
Used the [🎹 Spotify Tracks Dataset](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset), which includes tracks with features like `danceability`, `energy`, `loudness`, and `tempo`.  
**Preprocessing steps**:  
- 🧹 Removed redundant features  
- 🔠 One-hot encoded genres  
- 📏 Scaled numerical features using `StandardScaler`  

---

## 🛠️ Approach  
1. **🔍 Exploratory Data Analysis (EDA)**  
   Cleaned data and visualized feature distributions to understand the dataset.  

2. **🤖 Modeling with K-Means**  
   - Trained multiple K-Means models with varying `k` values.  
   - Used the **Elbow Method** (plotting SSE vs. clusters) to determine the optimal `k=10`.  
   - Identified dominant genres per cluster (e.g., *pagode, sleep, pop-film, death-metal*).  

3. **📐 Cluster Validation**  
   - Evaluated clusters using **Silhouette Scoring** to ensure balanced size and cohesion.  
   - Found `k=7` and `k=10` as strong candidates.  

---

## 📊 Results  
### Recommendation Example: Testing "Without Me" by Eminem:
🎯 Top 3 recommendations:
1. **goosebumps** – Travis Scott
2. **Unforgettable** – French Montana, Swae Lee
3. **All The Stars** – Kendrick Lamar, SZA

All recommended songs were hip-hop tracks, aligning with the input song’s genre! 🎤

---

## 🚧 Limitations & Insights
- While genre consistency is achieved, tempo/rhythm differences might make songs feel less similar.
- The system is simple but functional—a solid foundation for future improvements!
