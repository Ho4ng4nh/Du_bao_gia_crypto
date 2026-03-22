# Du_bao_gia_crypto
# Crypto Data Mining Pipeline

An automated data mining system that analyzes cryptocurrency market behavior using clustering and association rule mining.

This project builds a complete pipeline that processes historical crypto data, extracts financial indicators, discovers patterns between coins, and generates an easy-to-read analysis report.

---

## Project Overview

Cryptocurrency markets are highly volatile and complex.
This project applies **data mining techniques** to understand relationships between cryptocurrencies and group coins with similar behavior.

The pipeline automatically:

* Processes raw crypto price data
* Calculates key financial indicators
* Clusters cryptocurrencies based on risk and return
* Finds relationships between coin movements
* Generates a readable analysis report

---

## Data Mining Techniques Used

### 1. Feature Engineering

The system calculates important indicators such as:

* Return (price change)
* Volatility (risk level)

These metrics help measure the behavior of each cryptocurrency.

---

### 2. Clustering (K-Means)

Cryptocurrencies are grouped into clusters based on:

* Average return
* Volatility

This allows the system to identify:

* High-risk coins
* Medium-risk coins
* More stable coins

Example insight:

* Bitcoin tends to appear in a low volatility cluster
* Altcoins like Dogecoin show higher volatility

---

### 3. Association Rule Mining (Apriori)

The project uses Market Basket Analysis to detect relationships such as:

If one coin increases or decreases, another coin may behave similarly.

Metrics used:

* Support
* Confidence
* Lift

This helps discover hidden patterns in the crypto market.

---

## Project Structure

```
DATA_MINING_PROJECT
│
├── data
│   └── crypto_dataset.csv
│
├── scripts
│   └── run_pipeline.py
│
├── src
│   ├── features
│   │   └── build_features.py
│   │
│   ├── mining
│   │   ├── clustering.py
│   │   └── association.py
│   │
│   ├── visualization
│   │   └── plot_clusters.py
│   │
│   └── report
│       └── generate_report.py
│
├── outputs
│   ├── cluster_plot.png
│   ├── association_rules.csv
│   └── analysis_report.txt
│
└── README.md
```

---

## How to Run the Project

Clone the repository

```
git clone https://github.com/yourusername/crypto-data-mining.git
cd crypto-data-mining
```

Install dependencies

```
pip install -r requirements.txt
```

Run the pipeline

```
python scripts/run_pipeline.py
```

---

## Output Results

After running the pipeline, the system will generate:

Cluster Visualization

* A plot showing how cryptocurrencies are grouped

Association Rules

* Relationships between coin movements

Automated Analysis Report

* A readable summary of the market insights

Example outputs:

```
outputs/
│
├── cluster_plot.png
├── association_rules.csv
└── analysis_report.txt
```

---

## Example Insights from the Model

The system can automatically identify:

* Which cryptocurrencies are the most volatile
* Which coins behave similarly
* Which assets are relatively stable
* Possible relationships between market movements

Example finding:

Bitcoin tends to be more stable compared to other cryptocurrencies, while some altcoins exhibit higher volatility.

---

## Technologies Used

Python
Pandas
Scikit-learn
Mlxtend
Matplotlib

---

## Future Improvements

Possible upgrades for this project:

* Interactive dashboard (Streamlit)
* Real-time crypto data integration
* Advanced clustering evaluation
* Portfolio risk analysis
* Market prediction models

---

## Author

Hoàng Anh
Data Mining Project
