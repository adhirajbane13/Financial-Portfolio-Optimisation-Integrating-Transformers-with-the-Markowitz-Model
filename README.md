# Financial Portfolio Optimization Integrating Transformers with the Markowitz Model

## Description
This repository details an advanced financial model combining Transformer neural networks with the classical Markowitz Portfolio Optimization to enhance investment strategies for small-cap stocks indexed to Russell 2000. By leveraging Azure Databricks for heavy computational tasks, this approach overcomes the traditional model limitations by harnessing machine learning capabilities to capture dynamic and non-linear market patterns, thereby significantly improving financial portfolio management.

## Repository Structure
- `Codes/`: Jupyter notebook developed and executed in the Azure Databricks environment.
- `Outputs/`: Includes files like charts and visualizations generated from the scripts. Key files include:
  - `model_perf.png`: Visualization of the model's performance metrics.
  - `pbi_dashb.png`: PowerBI dashboard screenshot showing comprehensive visualization outcomes.
  - `pc_trans.png` & `pc_wotrans.png`: Charts comparing portfolio compositions with and without Transformer integration.
  - `ret-risk.png`: Returns vs. risk analysis graph.
  - `returns_curve.png`: Graph showing the returns curve over the simulation period.

## Installation and Setup
Ensure you have the following libraries installed to set up the necessary environment on Azure Databricks:
- TensorFlow 2.x
- Pandas
- NumPy
- Matplotlib
- SciPy
- yfinance

To install the required libraries:
```bash
%pip install tensorflow pandas numpy matplotlib scipy yfinance
```

## Key Components
1. **Data Collection**: Automated fetching of historical adjusted closing prices for Russell 2000 index stocks from July 1, 2021, to July 1, 2024, using `yfinance`.
2. **Data Preprocessing**: Includes data cleaning, normalization, and sequence generation for input to the Transformer model—all conducted on Azure Databricks.
3. **Transformer Model Training and Evaluation**: Extensive training and evaluation of the deep learning model to forecast future stock returns accurately.
4. **Portfolio Optimization**: Application of forecasted returns within the Markowitz framework to determine optimal asset allocation.
5. **Visualization of Results**: Utilizes Matplotlib for static plots and integrates with PowerBI for dynamic, interactive dashboard visualizations of optimized portfolio performances.

## Detailed Results
The integrated approach demonstrated a substantial improvement in portfolio performance:
- **Return Improvement**: Achieved approximately 1.4 times higher returns than the baseline Markowitz model.
- **Risk Reduction**: Reduced portfolio risk by about 15%, compared to traditional strategies.

These results are visualized in detailed charts and dashboards included within the `Outputs/` directory, providing clear evidence of the model's effectiveness in dynamic market conditions.
