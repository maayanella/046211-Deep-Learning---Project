# NBA Game Winner Prediction
Welcome to the NBA game winner Prediction project repository.


## Overview
In this project, we aim to use historical data from the past few decades to predict the winners of future games. Specifically, we want to determine which team is likely to win the next match based on past games data.


## Methodology
We aimed to predict the winner of a NBA gma by using 3 main ML predictors, Logistic Regression, XGBoots and CNN. The input of the predictions tools is a collection of previous games of both opponents and their last matchups. 


## Data
The dataset used in this project was sourced from Kaggle and encompasses game statistics spanning from the 1960s to 2023. Initially, we filtered the raw data to include only games with complete statistical lines. This filtering process resulted in a dataset of approximately 45,000 games, categorized into ‘Regular Season’ and ‘Playoffs’ games. The dataset exclusively contains team statistics, such as shot attempts, rebounds, fouls, and other metrics, without any individual player statistics. To prepare the data for analysis, we applied a normal distribution to each column. Additionally, we created a collection of previous games for each row, as previously mentioned.

<img width="1330" alt="image" src="https://github.com/user-attachments/assets/50ca81a5-8cd0-4202-8b1a-e37446496491">

## Model
RWKV is often used for NLP (natural language processing) tasks, but since our project does not focus on NLP, we had to adjust it. Therefore we added a few layers as can be seen in the diagram below.
![Screenshot 2024-04-07 222219](https://github.com/DanielLevi6/046211-Deep-Learning/assets/88712194/c4901f7e-f8c9-4b31-9d58-10795da04ea7)


## Repository Structure
- **data:** This directory contains datasets used for training, validating, and testing the prediction model.
- **code:** Source code for the prediction model implementation is located here.
- **results:** This directory stores model predictions and relevant visualizations.


## How to Use
To utilize our earthquake prediction model, follow these steps:
1. **Clone the Repository:** Clone this repository to your local machine.
2. **Install Dependencies:** Ensure all necessary dependencies are installed.
3. **Prepare Data:** If using custom data, format it appropriately and replace the existing dataset.
4. **Run the Model:** Execute provided scripts in the `code` directory.
5. **Evaluate Results:** Examine predictions and evaluate model performance.

## Libraries Used

| Library              | Command to Install                   |
|----------------------|--------------------------------------|
| transformers         | `pip install transformers`           |
| rwkv                 | `pip install rwkv`                   |
| numpy                | `pip install numpy`                  |
| pandas               | `pip install pandas`                 |
| torch                | `pip install torch`                  |
| matplotlib           | `pip install matplotlib`             |
| tqdm                 | `pip install tqdm`                   |
| sklearn.metrics      | `pip install scikit-learn`           |

## Results Summary
Our adapted RWKV method shows good results in predicting the number of earthquakes in Turkey. We used training, validation, and testing to achieve our results. Detailed results and visualizations can be found in the `results` directory. While our predictions did not match the magnitude's full size, it successfully predicted spikes when they occurred.
![WhatsApp Image 2024-04-07 at 21 04 28_e8f44de1](https://github.com/DanielLevi6/046211-Deep-Learning/assets/88712194/943feeb5-5404-42fb-9433-4372b0844a0b)


## Conclusion
In conclusion, our project demonstrates the effectiveness of utilizing advanced numerical techniques, such as RWKV, for earthquake prediction tasks. By leveraging methodologies tailored to our specific requirements and leveraging the resources available at the Technion, we have made significant strides toward enhancing our understanding and forecasting capabilities of seismic events in Turkey.


## References
- Kaggle dataset website - https://www.kaggle.com/datasets/ozgecinko/turkey-earthquake-data-1914-2023
- Hugging face RWKV - https://github.com/younesbelkada/transformers/tree/b4d4d6fe87ffcd7508307970cdf8fa3eda288701/src/transformers/models/rwkv


## Future Work
While our current model shows good results, there is still room for improvement. Future work could focus on further fine-tuning the model parameters, incorporating additional data sources, and exploring alternative prediction algorithms to enhance accuracy and robustness.
Additionally, more data features can be used and implemented in the model such that it will improve the model's capabilities of predicting the number of earthquakes.

## Contact
For inquiries or further information, please contact danielevi@campus.technion.ac.il, tzvi-tal@campus.technion.ac.il

Thank you for your interest in our Earthquake Prediction project.
