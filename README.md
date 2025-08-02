# VideoGameRevenueEstimator

Overview:
This project is applicable for independent and indie developers to estimate the revenue their game is likely to generate based on public data using real titles. This project uses a few predictive models to minimize the necessity for guesswork or intuition regarding target audience reception and price among other factors.

Dataset:
- Source: Game-Stats.com (https://www.games-stats.com)
- Data Size: 81,539 total titles
- Key Metrics:
      Price: (USD) Steam Marketplace Listing price
      Reviews: Total amount of user ratings
      Followers: Game developers' follower count
      Score: User-Generated Rating (Values ranging 1-10)
      Net Revenue: (USD) Target variable - total revenue generated from sales.

  Machine-Learning Models:
    Linear Regression   -   For interpretability of data
    Ridge Regression    -   For multicollinearity
    Lasso Regression    -   Feature selection and feature impact analysis
    Logistic Regression -   Binary result for feasability of revenue (Will the game generate a revenue higher than 67,000?)

  Evaluation Metrics:
  R^2
  Mean Absolute Error (MAE)
  Mean Squared Error (MSE)

  Results/Findings:
    Reviews consistently showed the strongest influence on net revenue (R^2 of 0.76)
    Lasso Regression helped cross-check findings, pinpointed strong and weak predictors
    Logistic Regression assisted with recognizing high-earning and low-earning games with an 84.7% accuracy
    Each regression model had unique takes and allowed us to understand the data better in their own right.

  Libraries and Tools Used:
    Language: Python 3.12
    Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn
    Development Tools: Google Colab, GitHub

  Instructions:

  1. Clone Repo -    [git clone https://github.com/(username)/video-game-revenue-predictor.git]

  2. Run Notenbook - open the [project_cleaned.ipynb] notebook in an appropriate reader such as Jupyter or Google Colab
 

  Folder Structure:

  >>group_7
  >>    source_code
  >>        project_cleaned.ipynb
  >>    data
  >>        Steam-Data.csv
  >>        Steam-Data.xlsx
  >>
  >>    readme.txt
  


Contributors:

  Allen Jean, Alvaro Flores, Hayden Heninger, Vinicius Intravartola
  
