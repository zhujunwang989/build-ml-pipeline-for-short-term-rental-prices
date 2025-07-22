# Build an ML Pipeline for Short-Term Rental Prices in NYC
You are working for a property management company renting rooms and properties for short periods of 
time on various rental platforms. You need to estimate the typical price for a given property based 
on the price of similar properties. Your company receives new data in bulk every week. The model needs 
to be retrained with the same cadence, necessitating an end-to-end pipeline that can be reused.


## 🔗 Project Links

- **GitHub Repository**: [build-ml-pipeline-for-short-term-rental-prices](https://github.com/zhujunwang989/build-ml-pipeline-for-short-term-rental-prices.git)
- **W&B Dashboard**: [NYC Airbnb Experiment Tracking](https://wandb.ai/wangzhujunshine-georgia-tech-alumni-association/nyc_airbnb?nw=nwuserwangzhujunshine)


## ⚙️ Tools Used

- **Hydra**: configuration management
- **MLflow**: experiment tracking & orchestration
- **W&B (Weights & Biases)**: artifact versioning & model evaluation
- **Scikit-learn**: model training (Random Forest)
- **Pandas**: data manipulation
- **Python 3.10**

## 🧪 Pipeline Steps

1. **Download** raw CSV data and log it to W&B
2. **Basic Cleaning**: remove outliers, handle nulls
3. **Data Check**: integrity & distribution checks
4. **Train/Val/Test Split**
5. **Model Training**: Random Forest regression
6. **Model Evaluation**: Run on test set, log metrics to W&B

Each step is modular and orchestrated via `mlflow.run()` inside `main.py`.

