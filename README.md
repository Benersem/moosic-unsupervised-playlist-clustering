# Moosic: Playlist Clustering Using Unsupervised Machine Learning

Welcome to **Moosic**, a project developed to assist a growing music startup in automating playlist creation using unsupervised machine learning techniques.

## 🎧 Project Background

Moosic curates expert-made playlists that resonate with specific moods and styles. However, as their user base expands, manually crafting playlists is becoming unsustainable. This project leverages **Spotify's audio features** and **unsupervised learning algorithms** to prototype a system that groups similar songs — effectively laying the groundwork for automated playlist creation.

---

## 📊 Objective

- Use **clustering algorithms** (e.g., K-Means) to group songs based on Spotify audio features.
- Evaluate the extent to which these features reflect perceived musical “moods” or styles.
- Explore the potential of **dimensionality reduction (PCA)** for better visualization and interpretation.
- Determine whether K-Means is sufficient, or if future iterations should consider alternative algorithms (e.g., DBSCAN, hierarchical clustering).

---

## 📁 Project Structure

| Folder/File            | Description |
|------------------------|-------------|
| `data/`                | Contains the datasets (`10_songs.csv`, `5000_songs.csv`) from Spotify API. |
| `notebooks/`           | Jupyter Notebooks used for data exploration, feature scaling, clustering, and visualization. |
| `images/`              | Cluster maps, PCA visualizations, and plots. |
| `src/`                 | Python scripts for preprocessing, clustering functions, and PCA utilities. |
| `presentation/`        | Final slides for presenting findings and insights. |
| `requirements.txt`     | Python dependencies. |
| `.gitignore`           | Standard Git ignore settings for Jupyter notebooks, Python cache, etc. |

---

## 🧪 Features Used from Spotify

This project uses a selection of audio features available via the Spotify API:

- `acousticness` — confidence that the track is acoustic
- `danceability` — suitability for dancing
- `energy` — perceptual intensity and activity
- `instrumentalness` — likelihood of no vocals
- `valence` — musical positiveness
- `tempo` — beats per minute
- `liveness`, `loudness`, `key`, `mode`, `speechiness`, `duration_ms`, `time_signature`

![radar_chart](https://github.com/user-attachments/assets/ac3f6d99-3e1a-4c2f-b1a7-88d2bfb723f5)

---

## ⚙️ Methods and Techniques

- **Feature Scaling**: MinMaxScaler, RobustScaler, PowerTransformer
- **Clustering**: K-Means
- **Evaluation**: Elbow method, Silhouette score
- **Dimensionality Reduction**: PCA
- **Visualization**: Seaborn, Matplotlib, Plotly (for interactive plots)

---

## 💡 Key Questions Explored

- Do Spotify’s audio features capture human-like understanding of song similarity?
- Can clustering algorithms like K-Means produce meaningful playlists?
- What are the limitations of the current approach, and how can we improve it?

---

## 🛠 Installation

```bash
git clone https://github.com/Benersem/moosic-unsupervised-playlist-clustering.git
cd moosic-unsupervised-playlist-clustering
pip install -r requirements.txt
