# Project

Gold Price Prediction Using DQN and Active Feature Elicitation
Objective

The objective of this project is to predict gold prices using a combination of Reinforcement Learning (specifically Deep Q-Networks, DQN) and Active Feature Elicitation. The goal is to select the most relevant features dynamically and use them to build an accurate predictive model.
Dataset

The dataset includes various financial indicators and technical metrics such as 'Open', 'High', 'Low', 'Close', 'Adj Close', 'Volume', and several other market indices and trends. The 'Close' price is the target variable for prediction.
Key Steps

    Data Loading and Preprocessing
        Load the dataset, handle missing values, and convert categorical features to numeric using one-hot encoding.
        Split the data into initial observed and unobserved sets for the Active Feature Elicitation process.

    

    Active Feature Elicitation with DQN
        Implement a custom environment for feature selection using Gymnasium.
        Train a DQN agent to dynamically select the most relevant features based on their impact on model performance.
        The selected features are then used to update the model iteratively.

    Model Training and Evaluation
        Use the selected features to train a RandomForestRegressor to predict the 'Close' price of gold.
        Evaluate the model using Mean Absolute Error (MAE) to ensure the accuracy of predictions.

    Predicting Future Prices
        Simulate future data points and use the trained model to predict gold prices for the next 5 months.
        Visualize the predictions to analyze the model's performance over time.

Tools and Technologies

    Python: Programming language used for data processing, model training, and evaluation.
    Pandas: For data manipulation and preprocessing.
    Gymnasium: For creating a custom environment for reinforcement learning.
    Stable Baselines3: For implementing and training the DQN agent.
    Scikit-learn: For machine learning model implementation (RandomForestRegressor).
    Matplotlib: For data visualization.

Results

The project demonstrated the feasibility of using Active Feature Elicitation with DQN to dynamically select relevant features for gold price prediction. The model achieved a satisfactory level of accuracy, with Mean Absolute Error used as the evaluation metric. The future predictions showed the model's capability to forecast gold prices based on selected features.
Conclusion

This project showcases an innovative approach to financial forecasting by integrating reinforcement learning and feature selection. Active Feature Elicitation proved to be effective in selecting relevant features dynamically, leading to an accurate predictive model for gold prices. The use of DQN in this context highlights the potential of reinforcement learning in financial data analysis and feature selection.
