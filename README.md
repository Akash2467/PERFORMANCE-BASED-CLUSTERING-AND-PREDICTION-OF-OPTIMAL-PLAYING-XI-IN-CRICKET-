# PERFORMANCE-BASED-CLUSTERING-AND-PREDICTION-OF-OPTIMAL-PLAYING-XI-IN-CRICKET

This project applies machine learning techniques to analyze cricket players' performance data across formats (Test, ODI, T20), cluster them based on statistical metrics, rank them using a supervised model, and generate an optimal Playing XI. The end-to-end process includes data preprocessing, exploratory data analysis (EDA), clustering (K-Means), and ranking (Random Forest).

## Project Files

- `01_data_cleaning.ipynb` – Preprocessing and cleaning of raw cricket data  
- `02_eda_teamwise.ipynb` – Exploratory analysis of team-wise statistics  
- `03_eda_playerwise.ipynb` – Exploratory analysis of player-wise performance  
- `04_clustering.ipynb` – K-Means clustering of players  
- `05_ranking_and_playing11.ipynb` – Ranking players and generating Playing XI  
- `06_final_combined.ipynb` – Combined notebook with clustering and ranking logic  

## Objectives

- Clean and preprocess cricket datasets (batting, bowling, and fielding)
- Analyze team-wise and player-wise performance patterns
- Group players into clusters based on performance metrics
- Rank players using Random Forest based on weighted scoring
- Generate an optimal Playing XI for a given format

## Tools and Technologies

- Python
- Jupyter Notebook
- Pandas, NumPy for data handling
- Matplotlib, Seaborn for visualization
- Scikit-learn for clustering and model building

## Project Highlights

| Task                      | Metric / Result         |
|---------------------------|--------------------------|
| ODI Batting Clustering    | Silhouette Score: 0.65   |
| T20 Bowling Clustering    | Silhouette Score: 0.41   |
| T20 Batting Rank Accuracy | 80%                      |
| T20 Bowling Rank Accuracy | 80%                      |
| T20 Fielding Rank Accuracy| 91%                      |

- Player roles were segmented into top performers, average performers, and underperformers
- Optimal teams were generated using a combination of clustering and ranking

## Dataset Source

This project uses publicly available cricket datasets from Kaggle. You can download the raw data from the following link and place it in the same folder as the notebooks:

- [ICC Cricket Dataset – Kaggle](https://www.kaggle.com/datasets/mahendran1/icc-cricket)

> Note: The uploaded notebooks assume the data is locally available in the same directory. Please adjust paths if necessary.

## Future Work

- Incorporate additional features such as home/away performance, opposition stats, and recent form
- Build a user-friendly application using Streamlit or Gradio
- Extend the model to franchise-based leagues like IPL
- Try advanced ensemble models or contextual ranking algorithms
