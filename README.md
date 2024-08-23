# Earthquake Prediction in Turkey
Welcome to the Earthquake Prediction project repository.
This repository houses the code and resources for predicting the number of earthquakes in Turkey on a given day. Our main goal is to provide a reliable tool for forecasting seismic activity, aiding in disaster management and mitigation efforts.


## Overview
Earthquakes present significant challenges to communities and infrastructure, emphasizing the importance of accurate prediction. Our project focuses on forecasting the number of earthquakes occurring in Turkey within a specified time frame. By analyzing historical seismic data and employing predictive modeling techniques, we aim to provide valuable insights into earthquake occurrence patterns.


## Methodology
In this project, we adapted the Receptance, Weight, Key, and Value (RWKV) method to suit our numerical prediction task. RWKV is a powerful technique commonly used in time-series forecasting, which we modified and fine-tuned to suit our specific application better. Leveraging the expertise and resources available, we customized the algorithm to optimize its performance for earthquake prediction.


## Data
The dataset utilized in this project was obtained from Kaggle and comprises earthquake records about Turkey and its surrounding regions. Spanning from September 1994 to September 2023, the dataset exclusively encompasses earthquakes with magnitudes exceeding 3.0 on the Richter scale. Each earthquake record includes essential information such as the date and time of occurrence, latitude and longitude coordinates, depth below the Earth's surface, and various magnitude measurements (e.g., Richter scale, moment magnitude scale). Additionally, the dataset provides information on the type or source of the earthquake and specifies the location or geographical region where it occurred. This comprehensive dataset serves as the foundation for our earthquake prediction model, enabling robust analysis and forecasting of seismic activity within the region.
<br>
<br>

![WhatsApp Image 2024-04-07 at 21 04 28_e74cb264](https://github.com/DanielLevi6/046211-Deep-Learning/assets/88712194/c96e8a3b-c3f8-4f27-8d41-56e13096ba48)

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
