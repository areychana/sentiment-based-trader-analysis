# Sentiment-Based Trader Analysis

A data science project that analyzes sentiment data to provide insights for trading decisions.

## Overview

This project leverages sentiment analysis techniques to evaluate market sentiment and generate trading signals. It combines data analysis, visualization, and machine learning to help traders make informed decisions.

## Features

- **Sentiment Analysis**: Process and analyze sentiment data from various sources
- **Data Visualization**: Interactive charts and visualizations for market insights
- **Trading Signals**: Generate actionable trading recommendations based on sentiment trends
- **Statistical Analysis**: Comprehensive statistical evaluation of sentiment patterns

## Project Structure

```
sentiment-based-trader-analysis/
├── README.md
├── .gitignore
├── data/                    # Data files
├── notebooks/               # Jupyter notebooks for analysis
├── src/                     # Source code modules
└── results/                 # Output and results
```

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook
- pandas, numpy, scikit-learn, matplotlib, seaborn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/areychana/sentiment-based-trader-analysis.git
cd sentiment-based-trader-analysis
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/Scripts/activate  # On Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

### Usage

Open the Jupyter notebooks in the `notebooks/` directory to explore the analysis:

```bash
jupyter notebook
```

## Key Findings

### 1. Sharpe-like Ratio Across Sentiment Regimes

Our analysis reveals significant variations in risk-adjusted returns across different sentiment regimes:

- **Extreme Greed**: Highest median Sharpe-like ratio (~400), indicating strong performance during periods of extreme optimism. However, exhibits high volatility with outliers reaching 1000+.

- **Extreme Fear**: Lower median Sharpe-like ratio (~100), suggesting subdued returns during panic periods, though with relatively stable performance.

- **Fear**: Moderate performance with median ratio around 150-250, showing consistent but modest returns during fearful market conditions.

- **Greed**: Median ratio around 300, indicating good performance during bullish sentiment with moderate variability.

- **Neutral**: Lowest median ratio (~100), suggesting that neutral sentiment periods produce the weakest risk-adjusted returns.

- **Unknown**: Minimal or negligible performance contribution.

### 2. Total Profit & Loss (PnL) by Market Sentiment

The PnL analysis demonstrates profitability variations across sentiment regimes:

- **Extreme Greed & Fear**: Show highest variability with some trades reaching 1M+ in profits, indicating high-risk, high-reward scenarios.

- **Fear & Greed**: More stable median PnL around 0.05-0.10M with controlled volatility, offering balanced risk-reward profiles.

- **Extreme Fear**: Lower median PnL but with notable positive outliers, suggesting occasional significant wins despite generally modest returns.

- **Neutral & Unknown**: Clustered near zero, confirming minimal profit generation in these sentiment regimes.

### 3. Win Rate by Sentiment Regime

Trade success rates vary significantly by sentiment:

- **Extreme Greed**: 35-60% win rate with some trades achieving 90%+ success, showing strong performance potential.

- **Extreme Fear**: 25-42% win rate, indicating lower success rates but with occasional high-performing trades (up to 100%).

- **Fear**: 15-70% win rate with broader range, showing more inconsistent results.

- **Greed**: 35-82% win rate, demonstrating relatively consistent and reliable trading performance.

- **Neutral**: 40-75% win rate, comparable to other regimes despite lower absolute returns.

### Trading Implications

- **Extreme Greed periods** offer the highest risk-adjusted returns but require careful risk management due to volatility
- **Greed regimes** provide the most reliable win rates and consistent profitability
- **Neutral sentiment** periods should be approached cautiously with conservative strategies
- **Fear-based regimes** provide opportunities for high-reward trades but with lower consistency
- **Portfolio diversification** across sentiment regimes can help balance risk and return

## Technologies Used

- **Python**: Core programming language
- **Pandas**: Data manipulation and analysis
- **Scikit-learn**: Machine learning models
- **Matplotlib/Seaborn**: Data visualization
- **Jupyter Notebook**: Interactive analysis

## Author

Archana Kumari

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For questions or suggestions, feel free to reach out!