📈 AI-Powered Financial Forecasting + LLM Reddit Sentiment Analysis
🧠 Project Overview
This project combines two powerful applications of artificial intelligence:

Stock Price Forecasting: Using advanced ML models (XGBoost) and financial indicators to predict short-term market movements across tech stocks.

Sentiment Analysis on Bitcoin Subreddit: Leveraging GPT-based large language models (LLMs) to analyze user sentiment from Reddit posts related to Bitcoin.

🔍 Part 1: AI-Powered Stock Forecasting
✅ Data Sources
Historical price, volume, and technical indicators for major tech stocks.

Company metadata (tickers, industry sectors).

Risk metrics: Put/Call ratios, risk scores from external CSVs.

⚙️ Modeling Approach
XGBoost Classifier with binary targets: "Up" or "Down".

Features include:

SMA, RSI, VIX, Momentum, Volatility

VolumeBreadth, PriceStrength

Custom engineered indicators

🔄 Forecasting Framework
Multi-horizon prediction (1, 3, 5, 10, 15, 20 days).

Evaluation metrics:

Accuracy

Up/Down Precision

Feature importance analysis per stock per horizon.

📊 Outputs
📈 Accuracy trends across horizons

🔍 Feature importance visualizations

🧭 Forward-looking directional summaries

🛡️ Confidence-based classification ("Up", "Down", "Low Confidence")

<p align="center"> <img src="img/accuracy_horizon.png" width="700"><br> <em>Accuracy across forecasting horizons</em> </p>
💬 Part 2: Reddit Sentiment Analysis Using LLM
🧾 Data
~120 user posts scraped from the Bitcoin subreddit.

Fields: title, post_text, timestamp, URL.

⚙️ Method
GPT-3.5-turbo used via OpenAI API.

Prompt-based classification into: Positive, Negative, or Neutral.

Custom Python pipeline with OpenAI's new SDK v1.0.

📊 Output
Sentiment distribution bar plot.

Insight into emotional tone of the crypto community.


