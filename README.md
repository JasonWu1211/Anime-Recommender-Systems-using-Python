# Anime Recommender Systems | Python, Surprise, Jupyter

The goal of this project was to develop a collaborative-based anime recommender system capable of generating a personalized list of unique and relevent anime recommendations based on database information comprising total user history and rating ID user feedback.The source of the data is from Kaggle.com [(Anime dataset from Kaggle)](https://www.kaggle.com/CooperUnion/anime-recommendations-database). There are two associated datasets, rating dataset and anime dataset. The rating dataset contains 7,813,737 Ratings (Rating scale: 1- 10) from 73,516 users on 12,294 anime with a density of 0.92%; the anime dataset consists of information about each anime with 7 columns (anime_id, name, genre, type, episodes, rating, and members). Using, python surprise package and custom builed data cleaning and model evlauation & validation programs, I investigated different kind of collaborative filtering (CF) algorithms including item-based KNNWithMeans, SVD, Co-clustering, and SVDpp. 


![model comparison & evalaution](/graph/recQualityPlot3.png)


* Overall, SVD performed best on recommending ranked list of relevent anime for users based on nDCG (ranking accuracy metric) without sacrifing too much speed
* KNNWithMeans performed best on finding Niche listings


Scripts:
- Jupyter NoteBook
  1. [Exploratory Analysis](/Jupyter%20notebook/Jason_Anime_recommender_system-EDA_of_original_anime_datasets.ipynb)
  2. [Data Preproccesing](/Jupyter%20notebook/Jason_Anime_recommender_system_Data_Preproccessing.ipynb)
  3. [Model Training & Validation](/Jupyter%20notebook/Jason_Anime_recommender_system_Model%20training.ipynb)
  4. [Model Evaluation & Selection](/Jupyter%20notebook/Jason_Anime_recommender_system_Model%20Evaluation_and_Comparsion.ipynb)
- Python
