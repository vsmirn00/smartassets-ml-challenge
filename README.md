# Junior AI Engineer Technical Challenge

This challenge is designed to evaluate your technical skills, problem-solving abilities, and proficiency in developing and deploying AI-driven solutions. You will be tasked with creating a Machine Learning API for Time Series Forecasting.

## Description

Your task is to develop an application that uses machine learning to provide time series forecasting. You will start with exploratory data analysis, proceed to model selection and feature engineering, evaluate your model, and then deploy it as a FastAPI application. The final application should be containerized using Docker.

The dataset you will be working with is provided in the `data` folder, accompanied by a `dataset_description.md` file that describes the dataset in detail. The target variable is `sales`, and you have access to several features that may help you build a predictive model. The dataset is a time series, and you will be tasked with forecasting the sales for a given date and store. 

The project uses `poetry` as a package manager, however you are free to use whichever package manager you are comfortable with.

*As a stretch goal you can finalize the app found in the `app` folder, and build a docker image*
The application is built with `FastAPI` and The application is already scaffolded so the main focus should be on the machine learning model and the API development. You would need to adjust the code minimally to be able to run properly. 

## Instructions
Steps 1-4 are *_essential_* for the deliverable, and steps 5-6 are optional stretch goals.

1. **Exploratory Data Analysis (EDA):** Begin with an exploratory data analysis to understand the dataset's characteristics, including trends, seasonality, and any outliers or anomalies.
    - Analyze dataset trends, seasonality, outliters and anomalies. 
    - Recommended tools: Pandas and Matplotlib/Seaborn.
2. **Feature Engineering:** Create and select features that will help improve your model's predictive performance.
    - Generate features to enhance model predictive performance. Consider historical sales data, time components (e.g., day of week, month), and external factors (e.g., holidays).
    - There are no strict limits on the number or type of features, but aim for relevance and effectiveness.
3. **Model Selection:** Choose a suitable model for time series forecasting. Justify your choice.
    - Select a model suitable for time series forecasting (e.g., ARIMA, LSTM). Justify your choice based on the model's appropriateness for the data characteristics and forecasting goals.
    - Criteria for justification: accuracy, computational efficiency, and ease of interpretation.
    - Note: think about creating a *baseline* model to compare your model's performance.
4. **Model Training and Evaluation:** Train your model and evaluate its performance using appropriate metrics. Aim for a model that balances accuracy and efficiency.
    - Train your model and evaluate its performance using metrics like RMSE (Root Mean Squared Error) or MAE (Mean Absolute Error).
    - Seek a balance between accuracy and efficiency. Explain your approach in the documentation.

#### Stretch Goals:

5. **API Development:** Develop a FastAPI application that serves your machine learning model. The API should accept input parameters relevant to your model and return a forecast.
    - Scafolding has been done for the application, you should be able to go through the applicationa and understand the structure.
    - you can find the application in the `app` folder.
    - it can be run from the root folder of the challenge using the command `uvicorn app.main:app --reload` and it should be available at `http://127.0.0.1:8000/docs`
6. **Dockerization:** Containerize your FastAPI application using Docker. Provide a Dockerfile and detailed instructions on how to build and run the container.
    - Hint: you might want to use the following command to generate `requirements.txt` file: `poetry export --without-hashes --format=requirements.txt > requirements.txt`


## Deliverables
The deliverables are split into two: essential & stretch goals.

*Essential:*
1. A Jupyter notebook containing your EDA, feature engineering, model selection, and evaluation process.*(Note: be ready to present this notebook to the team during the interview process, you can also make a presentation of the notebook if you want to.)*
2. A README.md file that includes: 
    - An overview of your solution.
    - Instructions on how to run your solution (in the case of a notebook, you can provide instructions on how to run the notebook within the notebook).


*Stretch Goals:*
1. A FastAPI application codebase, including all necessary files for running the app.
2. A Dockerfile for containerizing your application.
3. A README.md file that includes:
   - Instructions on how to set up and run your application.

## Evaluation Criteria

Your submission will be evaluated based on:

- Code quality and organization.
- Effectiveness and creativity of your feature engineering and model selection.
- Performance of your machine learning model.
- Functionality and design of your FastAPI application.
- Completeness and clarity of your documentation.

## Submission

Please create a private Github repository with your solution, and share it with us.
- Eric Walzthöny eric.walzthony@smartassets.ai
- Andrey Nunez andrey.nunez@smartassets.ai
- Nathan Hotchkin nathan.hotchkin@smartassets.ai

## Deadline

Your complete submission is due 4 days after receiving the technical challenge . Late submissions may not be considered for evaluation.

If you have any questions or need clarification on any aspect of the challenge, please feel free to reach out to:  Eric Walzthöny eric.walzthony@smartassets.ai.

Good luck, and we look forward to reviewing your innovative solutions!