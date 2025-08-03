# VideoGameRevenueEstimator

## Overview:
This project is applicable for independent and indie developers to estimate the revenue their game is likely to generate based on public data using real titles. This project uses a few predictive models to minimize the necessity for guesswork or intuition regarding target audience reception and price among other factors.

### Dataset:
- *Source:* [https://games-stats.com/steam/](Games-Stats.com)
- *Data Size:* 81,539 *total* titles 
- *Key Metrics:*
     -  <ins>Price:</ins> (USD) Steam Marketplace Listing price
     -  <ins>Reviews:</ins> Total amount of user ratings
     -  <ins>Followers:</ins> Game developers' follower count
     -  <ins>Score:</ins> User-Generated Rating (Values ranging 1-10)
     - <ins>Net Revenue:</ins> (USD) Target variable - total revenue generated from sales.

  ## Machine-Learning Models:
    *Linear Regression*   -   For interpretability of data
    *Ridge Regression*    -   For multicollinearity
    *Lasso Regression*    -   Feature selection and feature impact analysis
    *Logistic Regression* -   Binary result for feasability of revenue (Will the game generate a revenue higher than 67,000?)

  ### Evaluation Metrics:
  R²
  Mean Absolute Error (MAE)
  Mean Squared Error (MSE)

  ## Results/Findings:
    - Reviews consistently showed the strongest influence on net revenue (R² of 0.819)
    - Lasso Regression helped cross-check findings, pinpointed strong and weak predictors
    - Logistic Regression assisted with recognizing high-earning and low-earning games with an 84.7% accuracy
    - Each regression model had unique takes and allowed us to understand the data better in their own right.

  # Libraries and Tools Used:
    Language: Python 3.12
    Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn
    Development Tools: Google Colab

  ## Instructions:

  1. **Clone Repo** -    [git clone https://github.com/(username)/video-game-revenue-predictor.git]

  2. **Run Notebook** - open the [project_cleaned.ipynb] notebook in an appropriate reader such as Jupyter or Google Colab
  3. **Click *Shift+Enter* or Ctrl/Command+Enter to run each cell individually** - Cells must be run from the top-down. You may also click the "Run all" button in the commands panel to automatically run sequentially.
  4. **Expirement!** - Run any regression model you want and generate visuals to aid in interpretation. You can also change certain coefficients like alpha values to dampen or strengthen them against data - see what features impact your target data the most!
 

  Folder Structure:
  ```
  >>group_7
      source_code
          project_cleaned.ipynb
      data
          Steam-Data.csv
          Steam-Data.xlsx
  
      readme.txt
  ```


# Contributors:

  *Allen Jean, Alvaro Flores, Hayden Heninger, Vinicius Intravartola*
  
