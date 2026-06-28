# Trade & Ahead – Stock Clustering
An unsupervised machine learning pipeline utilizing K-Means and Hierarchical Clustering to segment equities based on financial health, volatility profiles, and performance metrics.

## Business Objective
Discover latent structural patterns within equity markets by grouping stocks with highly correlated financial characteristics. This pipeline automates asset tiering, separates high-risk from low-risk instruments, and provides data-driven insights to support portfolio diversification and risk analysis.

## Dataset Overview
- Number of Stocks: 340 
- Number of Financial Features: 11
- Industry: Equity Markets
- Learning Method: Unsupervised Learning

## Tech Stack & Advanced Libraries
* **Language:** Python
* **Data Engineering:** Pandas, NumPy
* **Machine Learning:** Scikit-learn (sklearn)
* **Statistical & Hierarchical Computation:** SciPy
* **Data Visualization:** Matplotlib, Seaborn

## Business Questions
- Can stocks be grouped based on similar financial characteristics?
- Which stocks exhibit high-risk versus low-risk behavior?
- Can clustering support portfolio diversification decisions?
- What hidden relationships exist across industries?

## Skills Demonstrated
- Unsupervised Machine Learning
- K-Means Clustering
- Hierarchical Clustering
- Feature Scaling
- Data Visualization
- Exploratory Data Analysis
- Financial Analytics
- Python
- Pandas
- NumPy
- Scikit-Learn
- SciPy
  
## Feature Matrix & Market Indicators
The unsupervised model processes multi-dimensional financial data points, including:
* **Financial Ratios:** Valuation, profitability, and operational leverage metrics.
* **Market Performance Metrics:** Historical price momentum, return distributions, and asset liquidity.
* **Risk Indicators:** Statistical volatility markers and systemic risk dimensions.

## Technical Workflow & Algorithmic Execution

### 1. Data Engineering & Statistical Prep
* **Outlier Mitigation:** Executed rigorous statistical outlier detection via Interquartile Range (IQR) / Z-score thresholds to prevent geometric skewing in cluster centroids.
* **Feature Scaling:** Applied Standardization (StandardScaler) to normalize varying financial units, ensuring distance-based algorithms weight all financial metrics equally.

### 2. Exploratory Data Analysis (EDA)
* Conducted multi-variable correlation mapping to identify collinear relationships among financial ratios.
* Built feature distribution profiles to analyze market data skewness before clustering.

### 3. K-Means Clustering Optimization
* Determined the mathematically optimal number of clusters ($K$) using the **Elbow Method** (Within-Cluster Sum of Squares) coupled with **Silhouette Analysis**.
* Executed centroid-based partitioning to segment equities into high-density behavioral zones.

### 4. Hierarchical Agglomerative Clustering
* Generated statistical proximity matrices using SciPy to construct structural **Dendrograms**.
* Evaluated bottom-up linkage criteria (Ward’s method) to map the continuous evolutionary relationships and corporate taxonomies across the stock universe.

## Key Analytical Insights & Portfolio Impact

### Cluster Model Evaluation & Hyperparameters
To determine structural cohesion and separation across the stock universe, both K-Means and Agglomerative pipelines were cross-evaluated using geometric and spatial metrics:
* **Optimal Architecture:** Final model convergence selected **$K = 4$ clusters**. 
* **Silhouette Score Metrics:** While the mathematical absolute maximum peak occurred at $K = 2$ ($\approx 0.45$), hyperparameter validation confirmed that $K = 4$ maintained a robust Silhouette Score of **0.42** while delivering significantly higher operational utility for asset managers.
* **Algorithmic Consistency:** Both K-Means distance matrices and SciPy bottom-up hierarchical linkage (Ward's method) consistently validated identical boundaries at 3 and 4 groupings.

### Core Market Discoveries & Portfolio Impact
* **Risk & Volatility Stratification:** The pipeline successfully isolated a distinct cluster of high-yield, hyper-volatile equities, cleanly separating them from low-beta, defensive blue-chip asset profiles.
* **Automated Asset Diversification:** The clustering model identified stocks with similar financial characteristics, helping investors build more diversified portfolios.
* **Investment Decision Support:** The clustering framework provides a data-driven approach to grouping stocks and reducing subjective investment decisions.

## Cluster Geometry & Visualizations
<img width="1716" height="228" alt="Screenshot 2026-05-27 161927" src="https://github.com/user-attachments/assets/2ba92b72-a6fe-4b00-ab7f-bfdd80255717" />
<img width="1184" height="684" alt="download" src="https://github.com/user-attachments/assets/732599dc-94b0-4c13-a3af-5ba6d1bdfba3" />
<img width="1547" height="117" alt="Screenshot 2026-05-27 162302" src="https://github.com/user-attachments/assets/0d18a153-3b39-4cf3-beaa-ac85e7a0e479" />
<img width="703" height="522" alt="download" src="https://github.com/user-attachments/assets/a1cc4e36-62ea-4abb-a7ac-5a004607949f" />





