# ESG Portfolio Performance Analysis

## Overview

This project analyzes the performance of portfolios based on Environmental, Social, and Governance (ESG) risk scores. Using the Capital Asset Pricing Model (CAPM) and the Fama-French Three-Factor Model, the project examines the risk-adjusted returns and volatility of top and bottom ESG portfolios. The analysis highlights the potential benefits of integrating ESG criteria into investment strategies.

## Table of Contents

- [Overview](#overview)
- [Table of Contents](#table-of-contents)
- [Data](#data)
- [Methodology](#methodology)
- [Results](#results)
- [Discussion](#discussion)
- [Files](#files)
- [Usage](#usage)
- [Acknowledgments](#acknowledgments)

## Data

The data used in this project includes:
- Stock prices and returns
- ESG risk scores for individual companies
- Fama-French factors

The cleaned combined stock and ESG data are stored in the file `SP 500 ESG Risk Ratings.csv`.

## Methodology

### Portfolio Construction

The cleaned combined stock and ESG data were used to create portfolios. The stocks were ranked based on their ESG scores, and the top and bottom 10% were selected to form the top and bottom portfolios, respectively, for each ESG component (Total ESG Risk score, Environment Risk Score, Social Risk Score, and Governance Risk Score).

### Performance Measurement

#### Capital Asset Pricing Model (CAPM)

The CAPM model was used to estimate the expected return on a portfolio relative to its risk compared to the market. The formula used is:

$ r_t = \alpha + \beta (R_m - R_f) + \epsilon_t $

#### Fama-French Three-Factor Model

The Fama-French model extends CAPM by including size and value factors. The formula used is:

$ r_t = \alpha + \beta_1 (R_m - R_f) + \beta_2 \text{SMB} + \beta_3 \text{HML} + \epsilon_t $

## Results

The analysis revealed significant differences in performance and risk characteristics between the top and bottom ESG portfolios. The results are summarized in the following tables:

- **Table 1: Characteristics of Portfolios**
  ![Table 1: Characteristics of Portfolios](Updated/Tables/1.Characteristics%20of%20Portfolios.png)
- **Table 2: The CAPM Regression Results**
  ![Table 2: The CAPM Regression Results](Updated/Tables/2.The%20CAPM%20Regression%20Results.png)
- **Table 3: Time Series Regression Results for ESG Portfolios**
  ![Table 3: Time Series Regression Results for ESG Portfolios](Updated/Tables/3.Time%20Series%20Regression%20Results%20for%20ESG%20Portfolios.png)
- **Table 4: Time Series Regression Results for ENV Portfolios**
  ![Table 4: Time Series Regression Results for ENV Portfolios](Updated/Tables/4.Time%20Series%20Regression%20Results%20for%20ENV%20Portfolios.png)
- **Table 5: Time Series Regression Results for SOC Portfolios**
  ![Table 5: Time Series Regression Results for SOC Portfolios](Updated/Tables/5.Time%20Series%20Regression%20Results%20for%20SOC%20Portfolios.png)
- **Table 6: Time Series Regression Results for GOV Portfolios**
  ![Table 6: Time Series Regression Results for GOV Portfolios](Updated/Tables/6.Time%20Series%20Regression%20Results%20for%20GOV%20Portfolios.png)

## Visualizations

The project includes various visualizations to help understand the data and results better. The visualizations can be found in the `Visualizations/` folder and include:

- ![Missing Values Heatmap Before Cleaning](Visualizations/1.Missing%20Values%20Heatmap%20Before%20Cleaning.png)
- ![Stock Prices Over Time](Visualizations/2.Stock%20Prices%20Over%20Time.png)
- ![Distribution of Total ESG Risk Scores](Visualizations/3.Distribution%20of%20Total%20ESG%20Risk%20Scores.png)
- ![Total Number of Stocks Analyzed Over Time](Visualizations/4.Total%20Number%20of%20Stocks%20Analyzed%20Over%20Time.png)
- ![Average ESG Risk Scores Over Time](Visualizations/5.Average%20ESG%20Risk%20Scores%20Over%20Time.png)
- ![Sector Representation in Top and Bottom Portfolios](Visualizations/6.Sector%20Representation%20in%20Top%20and%20Bottom%20Portfolios.png)
- ![Distribution of ESG Scores for Top and Bottom Portfolios](Visualizations/7.Distribution%20of%20ESG%20Scores%20for%20Top%20and%20Bottom%20Portfolios.png)
- ![Number of Stocks in Top and Bottom Portfolios Over Time](Visualizations/8.Number%20of%20Stocks%20in%20Top%20and%20Bottom%20Portfolios%20Over%20Time.png)
- ![ESG Scores for Different Risk Categories](Visualizations/9.ESG%20Scores%20for%20Different%20Risk%20Categories.png)
- ![Market Returns Over Time](Visualizations/10.Market%20Returns%20Over%20Time.png)
- ![Portfolio Returns Over Time](Visualizations/11.Portfolio%20Returns%20Over%20Time.png)

## Discussion

These findings are supported by the existing literature, which argues that ESG seems to be a positive driver of portfolio performance. This paper therefore adds to the literature as it supports the idea that not only do high ESG-scoring portfolios realize better risk-adjusted returns, but they also follow a lower volatility path. Furthermore, results back the notion that sustainable investing is financially beneficial.

These findings thereby underline the need to integrate ESG into the investment strategies for both investors and portfolio managers. On the other hand, high ESG scores go with high financial performance and low risk; thus, it shows the conclusion that sustainable investing is ethically not only desirable but also financially prudent. Hence, ESG criteria as one of the major components should form a construction of resilient and high-performing portfolios by the portfolio manager.

One of the central limitations of this research is that it looked at historical data, which may not be fairly representative of future trends and market conditions. Further, this paper focused on the S&P 500 Index; results may differ for other indices or regions. Further studies should grasp the influence of ESG factors across varied markets and sectors and test whether this dynamic relationship holds regarding ESG performance and financial returns over longer horizons.

## Files

### Main Directory

- `Assignment/`
- `Updated/`
- `Visualizations/`
- `DTB3.csv`
- `ESG_Portfolio_Performance_Analysis.ipynb`
- `F-F_Research_Data_Factors_daily.csv`
- `Impact of ESG Scores on Portfolio Performance.docx`
- `SP 500 ESG Risk Ratings.csv`

### Assignment Folder

- `ESGScoreonPOrtfolioperformance.pdf`
- `List Of Deliverables.pdf`
- `ResearchProposal-MAH.pdf`

### Updated Folder

- `ESG Data/`
  - `ESGCountry.csv`
  - `ESGCountry-Series.csv`
  - `ESGData.csv`
  - `ESGFootNote.csv`
  - `ESGSeries.csv`
  - `ESGSeries-Time.csv`
- `Tables/`
  - `1.Characteristics of Portfolios.png`
  - `2.The CAPM Regression Results.png`
  - `3.Time Series Regression Results for ESG Portfolios.png`
  - `4.Time Series Regression Results for ENV Portfolios.png`
  - `5.Time Series Regression Results for SOC Portfolios.png`
  - `6.Time Series Regression Results for GOV Portfolios.png`
- `ESG_Portfolio_Performance_Analysis.ipynb`
- `Impact of ESG Scores on Portfolio Performance.docx`

### Visualizations Folder

- `1.Missing Values Heatmap Before Cleaning.png`
- `2.Stock Prices Over Time.png`
- `3.Distribution of Total ESG Risk Scores.png`
- `4.Total Number of Stocks Analyzed Over Time.png`
- `5.Average ESG Risk Scores Over Time.png`
- `6.Sector Representation in Top and Bottom Portfolios.png`
- `7.Distribution of ESG Scores for Top and Bottom Portfolios.png`
- `8.Number of Stocks in Top and Bottom Portfolios Over Time.png`
- `9.ESG Scores for Different Risk Categories.png`
- `10.Market Returns Over Time.png`
- `11.Portfolio Returns Over Time.png`

## Usage

To run the analysis:

1. Ensure you have the necessary data files in the project directory.
2. Open the `ESG_Portfolio_Performance_Analysis.ipynb` Jupyter Notebook.
3. Follow the steps in the notebook to perform the analysis and generate results.
4. Review the results in the generated tables and graphs.

## Acknowledgments

- The data used in this project were sourced from reputable financial data providers.
- Special thanks to the contributors who provided valuable insights and guidance throughout the project.

## Disclaimer

This work is original and should not be used without proper attribution. Unauthorized use or plagiarism of this work is strictly prohibited. If you use this work, please provide proper credit to the author.

## Acknowledgments

- The data used in this project were sourced from reputable financial data providers.
- Special thanks to the contributors who provided valuable insights and guidance throughout the project.

