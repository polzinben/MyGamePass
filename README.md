# MyGamePass # 

With an estimated 1.2 Million (and growing!) games across all platforms today it can be overwhelming trying to find your next favorite game to play.  Using machine learning and natural language processing, MyGamePass intends to help solve this problem.

Situations for MyGamePass include:
- "I know I love this game (or games), how do I find more games like it?"
- "With so many options, I don't even know where to look.  What are people like me playing?"

I have built a rough prototype of a content based recommender system as well as a collaborative filtering system.

This project provides a great highlight of data analysis fundamentals as well as an understanding of more advanced concepts such as Machine Learning Pipelines as well as Natural Language Processing, Funk Singular Vector Decomposition, Cosine Similarity, and model evaluation.  Packages demonstrated include pandas, matplotlib, seaborn, sklearn, nltk, and surprise.  

---
## Prerequisites ##

The following packages are required in addition to python.  Please install at your own risk.

seaborn for visualizations:
`conda install seaborn`

scikit-learn for machine learning toolbox
`conda install scikit-learn`

Natural Language Toolkit for NLP
`conda install nltk`

Surprise library for matrix factorization and collaborative filtering:
`conda install -c conda-forge scikit-surprise`

Note - alternatively, MyGamePass.yml environment has been included in repository to clone from.

---
## Data Description ##

Two complementary datasets were acquired from Kaggle for this project.  The first dataset contains extensive game descriptive information from the steam store.  The second is a dataset containing 200,000 user-game interactions (purchase/play) from the steam store.

Steam Store Data
- `steam.csv` : Used as the master dataframe.  Contained store listing information for each game (name, release date, developer, genre, ratings, etc.) as well as the steam appid used for joining all tables
- `steam_description_data.csv` : Contained full text descriptions of each game used for NLP and content filtering
- `steam_users.csv` : 200,000 user-game interactions used for collaborative filtering

---
## File Directory ##
- `data` folder: stores all .csv files used in project acquired from Kaggle
    - `steam_store` : subfolder containing the steam store game descriptive data
- `deliverables` folder: stores summarizing documents
    - `ben_polzin_capstone_presentation` : presentation slides
    - `ben_polzin_capstone_report` : complete report of the project
- `1_steam_cleanup` : data analysis and preprocessing of master steam dataframe
- `2_descr_cleanup` : data preprocessing of steam game descriptions
- `3_user_cleanup` : EDA and preprocessing of user data
- `4_content_modeling` : content based recommender system using descriptive information
- `5_matrix_factorizatoin` : collaborative based filtering using Surprise library

---
### Thank you very much for your interest!  ### 
## Please reach out through LinkedIn for hiring inquiries. ##

linkedin.com/in/bpolzin

# END #
