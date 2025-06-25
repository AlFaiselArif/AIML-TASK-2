# Exploratory Data Analysis (EDA) Project

# Project Title
EDA on Movie Genre Classification Dataset

# Objective
The aim of this project is to perform Exploratory Data Analysis (EDA) on a movie dataset to:
- Understand its structure and key features.
- Generate meaningful statistical insights.
- Visualize data distributions and relationships.
- Identify trends, patterns, or anomalies.
- Make initial inferences that could help in further Machine Learning tasks.

# Dataset Description
- **Filename**:'C:/Users/alfai/Downloads/movie_genre_classification_final.csv'
- **Description**: This dataset contains various attributes of movies that could be used for genre classification and analysis.
-  Note: The original dataset is too large to preview on GitHub. A sample of 100 rows is available in `sample_movie_data.csv` for quick viewing.

# Key Columns in the Dataset:
Column Name   :  Description                                 
Genre         :  Primary genre of the movie                  
Duration      :  Duration of the movie (in minutes)          
Budget        :  Budget in USD                               
Gross         :  Gross earnings in USD                       
Votes         :  Number of votes received                    
Year          :  Year of release                             
Rating        :  IMDb rating of the movie                    
Metascore     :  Metacritic score of the movie               
Director      :  Director’s name                             
Cast          :  Names of main cast members                  
Certificate   :  Age rating certificate                      
Country       :  Country of origin                                                    
Language      :  Language of the movie                      

# Tools and Libraries Used
- *Python*
- Pandas – Data manipulation
- NumPy – Numerical operations
- Matplotlib – Static visualizations
- Seaborn – Enhanced statistical visualizations
- Plotly – Interactive visualizations (optional)

# Tasks Performed
 Summary Statistics
- Computed `mean`, `median`, `mode`, `standard deviation`, `min`, `max`, and other descriptive statistics for numerical features.

# Visualizations
- **Histograms** for distributions (e.g., `Duration`, `Rating`, `Gross`, `Votes`)
- **Boxplots** for outlier detection and spread
- **Correlation Matrix** and **Heatmaps** to identify multicollinearity
- **Pairplots** to examine feature-to-feature relationships

#Pattern & Trend Detection
- Identified which genres dominate the dataset.
- Found relationships between budget and gross income.
- Detected skewness in vote counts and gross earnings.
- Spotted anomalies (e.g., unusually high budget/low gross films).
  Patterns, Trends, or Anomalies Identified
-Distribution of Movie Ratings
Ratings are mostly clustered between 4.0 and 7.0, with a few higher-rated films.
A right-skewed distribution is visible, suggesting many average-rated movies, few high-rated ones.

-Boxplot of Budget
Several movies have budgets between 20M and 150M USD.
Outliers exist on the higher end (above 200M+), indicating a few big-budget films.
The presence of these high outliers can skew mean-based insights.

-Correlation Heatmap
Votes and BoxOffice show a strong positive correlation, implying that popular movies earn more.
Critic Reviews also correlate well with Votes and BoxOffice, indicating possible influence on viewership.
Budget and BoxOffice are moderately positively correlated, suggesting that higher investment often leads to better returns.

-Scatter Plot (Budget vs BoxOffice by Genre)
Action and Fantasy movies tend to have high budgets and high returns.
Drama and Romance cluster around lower budgets and returns, often more niche.
A few anomalies are seen:
-Some movies with very high budgets and low box office (likely commercial failures).
-Some movies with moderate budgets and exceptionally high returns (possibly sleeper hits).

#Feature-Level Inferences from Visuals
 Feature           Inference                      

 `Rating`           Most ratings fall in the average range; fewer exceptional ratings.          
 `Budget_USD`       High variance and outliers; investment strategies vary widely.              
 `BoxOffice_USD`    Influenced strongly by `Votes`, `Genre`, and `Budget`.                      
 `Votes`            Strong indicator of movie popularity and likely box office success.         
 `Genre`            Impacts both `Budget` and `BoxOffice`; Action/Fantasy often more invested.  
 `Critic_Reviews`   Correlates with `Votes`, suggesting critical praise aligns with popularity. 

