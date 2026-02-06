# primetradeAI-sentiment-analysis
# Data Analytics Intern – Round-0 Assignment (Trader Performance vs Market Sentiment)

This project analyzes the relationship between **Bitcoin market sentiment (Fear / Greed)** and **trader behavior & performance** using historical trading data from Hyperliquid.

The analysis is divided into:
- **Part A:** Data preparation & feature engineering  
- **Part B:** Performance, behavioral analysis & trader segmentation  

All analysis is executed using **Python cells inside VS Code**.

## Project Structure
primetradeAI-sentiment-analysis/
│
├── data/
│ ├── fear_greed_index.csv
│ └── historical_data.csv
|── outputs/
| 
|── report.md
├── sentiment_analysis.ipynb (VS Code cell-based)
├── README.md
└── requirements.txt

## Environment Setup

### 1. Prerequisites

- Python **3.8+**
- VS Code
- VS Code Extensions:
  - **Python**
  - **Jupyter** (for cell execution)

### 2. Installation
- Clone the repository

 - git clone https://github.com/Zunairafatima9/primetrade-assignment.git
 - cd primertade-assignment

### 3. Create and activate virtual environment (Recommended)

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate

# On Windows
python -m venv venv
venv\Scripts\activate

### 4. Install dependencies

pip install -r requirements.txt

### 5. Download datasets

- Download from the provided Google Drive links:
 - Bitcoin Market Sentiment
 - Historical Trader Data

- Place files in the data/ directory:
 - fear_greed_index.csv
 - historical_data.csv

###  How to Run the Analysis (VS Code Cells)

- Open analysis.py or analysis.ipynb in VS Code
- Ensure the correct Python interpreter / virtual environment is selected

- Run cells top to bottom using:
  - Shift + Enter (execute cell)

  - Follow the sections:
   - Load datasets
   - Data cleaning & alignment
   - Feature engineering
   - Sentiment-based analysis
   - Trader segmentation
   - Visualization & insights

# Methodology Overview

# Data Preparation
- Converted timestamps to daily granularity
- Removed duplicates and handled missing values
- Aggregated trade data per day and per trader

# Metrics Created
- Daily PnL per trader
- Win rate
- Trade frequency
- Long / short ratio
- Position exposure (Size USD as leverage proxy)

# Analysis Performed
- Performance comparison: Fear vs Greed
- Behavioral changes based on sentiment

# Trader segmentation:
- High vs Low exposure
- Frequent vs Infrequent traders
- Consistent vs Inconsistent traders

### Expected Outputs

After running the analysis, you'll find in the outputs/ directory:
- Visualizations (outputs):
  - performance_by_sentiment.png - Box plots comparing metrics
  - behavior_by_sentiment.png - Bar charts of trading behavior
  - correlation_matrices.png - Heatmaps of correlations
  - Segment analysis charts

- Reports:
  - summary_report.md - Executive summary with findings

###  Notes 

- Time Estimate: ~2.5 hours
- Data preparation: 45 min
- Analysis: 60 min
- Visualization: 30 min
- Documentation: 30 min

# Key Features:
- Handles actual column names from provided dataset
- Robust error handling for missing data
- Multiple visualization options
- Both notebook and script execution paths

