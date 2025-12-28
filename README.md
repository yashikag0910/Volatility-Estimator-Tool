Volatility Estimator & Event Impact Analysis
Overview
This project analyzes financial market volatility as a dynamic risk metric by computing and comparing multiple volatility estimators on the same asset. The analysis is performed in Google Colab, making the project fully reproducible without any local setup.
The project emphasizes how volatility evolves over time and how market uncertainty changes around major macroeconomic events such as CPI releases or central bank announcements.

Key Objectives
Analyze volatility as a time-varying risk measure
Compute and compare multiple volatility estimators
Study the effect of macroeconomic events on market risk
Visualize volatility regimes across different time horizons
Demonstrate financial and statistical intuition through interpretation


Methodology
1. Environment
Platform: Google Colab
Language: Python
2. Data Collection
Daily adjusted price data fetched using yfinance
Assets such as equities or indices (e.g., AAPL, SPY)
3. Return Calculation
Log returns computed from adjusted prices
Enables stable time-series analysis
4. Volatility Estimation
The following estimators are implemented:
Historical Volatility
Annualized standard deviation of log returns
Rolling Volatility
Time-varying volatility using rolling windows:
20 days (short-term)
60 days (medium-term)
120 days (long-term)
EWMA Volatility
Exponentially Weighted Moving Average volatility to emphasize recent market shocks
5. Event Impact Analysis
Selected macroeconomic events (e.g., CPI releases)
Volatility compared before and after the event window
Used to evaluate changes in market uncertainty


Results & Insights
Volatility exhibits clustering, confirming non-constant risk
Short rolling windows respond faster but introduce noise
Longer windows provide smoother, long-term risk estimates
EWMA volatility reacts more rapidly to sudden shocks
Macroeconomic events often trigger shifts in volatility regimes
These results reinforce that risk perception depends on model choice and market context.


How to Run (Google Colab)
Open Google Colab
Upload volatility_estimator.ipynb
Run all cells from top to bottom
All required libraries are installed automatically in the Colab environment.


Key Learnings
Volatility is dynamic, not static
Different estimators capture different aspects of risk
Macro events play a crucial role in uncertainty dynamics
Visualization is essential for interpreting market behavior


Future Improvements
Extend analysis to multiple assets or asset classes
Add GARCH-based volatility models
Automate macro event selection
Build an interactive dashboard for real-time analysis
