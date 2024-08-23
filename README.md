# NBA Game Winner Prediction
Welcome to the NBA game winner Prediction project repository.


## Overview
In this project, we aim to use historical data from the past few decades to predict the winners of future games. Specifically, we want to determine which team is likely to win the next match based on past games data.


## Methodology
We aimed to predict the winner of a NBA gma by using 3 main ML predictors, Logistic Regression, XGBoots and CNN. The input of the predictions tools is a collection of previous games of both opponents and their last matchups. 


## Data
The dataset used in this project was sourced from Kaggle and encompasses game statistics spanning from the 1960s to 2023. Initially, we filtered the raw data to include only games with complete statistical lines. This filtering process resulted in a dataset of approximately 45,000 games, categorized into ‘Regular Season’ and ‘Playoffs’ games. The dataset exclusively contains team statistics, such as shot attempts, rebounds, fouls, and other metrics, without any individual player statistics. To prepare the data for analysis, we applied a normal distribution to each column. Additionally, we created a collection of previous games for each row, as previously mentioned.

<img width="1330" alt="image" src="https://github.com/user-attachments/assets/50ca81a5-8cd0-4202-8b1a-e37446496491">

## Models
Logistic Regression is a linear model that can provide descent results only for simple problems and therfore used as baseline method for comparison. 
XGBoots model is more complex model, that use a decision tree with conrolable depth to predict. Althogt the XGBoots is more complex, it still has a limited span representation. 
The CNN model, is the complexiest, and the most fitable for out project goal. 

<img width="564" alt="image" src="https://github.com/user-attachments/assets/b6eefc7f-4dd2-49b7-ad00-559307348623">



## Repository Structure
- **data:** This directory contains raw datasets and the filtered dataset.
- **code:** Source code for the prediction model implementation is located here.


## How to Use
1. **Clone the Repository:** Clone this repository to your local machine.
2. **Install Dependencies:** Ensure all necessary dependencies are installed.
3. **Prepare Data:** If using custom data, format it appropriately and replace the existing dataset.
4. **Run the Model:** Execute provided scripts in the `code` directory.
5. **Evaluate Results:** Examine predictions and evaluate model performance.

## Libraries Used


| Library              | Command to Install                   |
|----------------------|--------------------------------------|
| numpy                | `pip install numpy`                  |
| pandas               | `pip install pandas`                 |
| torch                | `pip install torch`                  |
| matplotlib           | `pip install matplotlib`             |
| sklearn.metrics      | `pip install scikit-learn`           |
| xgboost              | `pip install xgboost`                |



## Conclusion & Results 
The CNN achieved the highest accuracy on the test set as expected.  XGBoost showed minimal improvement when optimizing hyperparameters or increasing input size. Logistic regression performed best with the smallest input size. The final and best results are summarized in the following table:


| Model          | CNN          | XGBoost  |      Logistic Regression     |
|----------------|--------------|---------------------|------------------|
| Accuracy       | 67%	| 60.33% 	| 58.69% |


<img width="388" alt="image" src="https://github.com/user-attachments/assets/1263def6-2200-4b4e-9a3f-992d72734350">


## References
- Kaggle dataset website - https://www.kaggle.com/datasets/wyattowalsh/basketball
- Previous work for example (1): https://github.com/luke-lite/NBA-Prediction-Modeling 
- Previous work for example (2): https://github.com/kyleskom/NBA-Machine-Learning-Sports-Betting
- Previous work for example (3): https://towardsdatascience.com/predicting-the-outcome-of-nba-games-with-machine-learning-a810bb768f20


## Future Work
Online models have shown marginally better performance than ours, even with basic techniques like XGBoost and logistic regression, or with CNN. While these differences are minimal, we believe there are two primary avenues for enhancing our model's accuracy.
First, increasing the input size has consistently led to improved predictions. However, we caution that excessive historical data could introduce noise. Moreover, this approach demands more computational resources and processing time.
Second, refining the data itself offers potential benefits. This could involve gathering additional game statistics, such as player-level data, or optimizing the preprocessing pipeline. We believe there is ample room for improvement in both areas.


## Contact
For inquiries or further information, please contact zilberman@campus.technion.ac.il, maayanella@campus.technion.ac.il

Thank you for your interest in our NBA Prediction project.
