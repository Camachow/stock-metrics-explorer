# Gerar o conteúdo do README.md como arquivo
readme_content = """
# 📊 Stock Market Analysis with Python

This project analyzes stock price variations using financial and company data from a multi-sheet Excel file. The analysis includes calculating daily returns, aggregating results by company segment, categorizing companies by age, and visualizing performance trends.

## 📁 Data Overview

The data is loaded from an Excel file containing four sheets:

- **Principal**: Daily stock prices and percentage variation.
- **Total_de_acoes**: Theoretical quantity of shares per stock.
- **ChatGPT**: Company metadata including age and category.
- **Ticker**: Mapping of tickers to company names.

## 🧪 Main Objectives

- Calculate real price variation (`R$`) for each stock based on daily percentage changes.
- Merge and enrich datasets with company metadata and theoretical quantity of shares.
- Classify stock performance as "Up", "Down", or "Stable".
- Categorize companies by age (`<50`, `50–100`, `>100` years).
- Analyze variations by business segment and performance outcome.
- Visualize results with interactive plots using Plotly.

## 🔧 Technologies Used

- **Python 3**
- **Pandas** for data manipulation
- **Plotly Express** for data visualization
- **Jupyter Notebook / Google Colab**

## 📈 Key Visualizations

- **Bar Chart**: Total variation in R$ grouped by performance outcome (`Subiu`, `Desceu`, `Estável`)
- **Pie Chart**: Sector distribution of stocks that gained value

## 🔍 Example Insights

- Biggest positive and negative price variations
- Average variation of stocks that went up vs. down
- Segments that contributed most to positive variations

## 🚀 How to Run

1. Clone this repository.
2. Open the Jupyter Notebook or run in Google Colab.
3. Make sure to upload the Excel file:  
   `Imersão Python - Tabela de ações.xlsx`
4. Run all cells sequentially to reproduce the analysis and charts.

## 📚 File Structure
├── ImersãoPython.ipynb # Main notebook with the full analysis
├── Imersão Python - Tabela de ações.xlsx # Required dataset (not included in repo)
└── README.md # Project documentation

## 🧠 Possible Extensions

- Add moving averages or other technical indicators
- Include historical time-series analysis
- Build an interactive dashboard (e.g., with Streamlit or Dash)

## 👨‍💻 Author

Made with 💻 by [Your Name] – feel free to connect or contribute!

## 📄 License

This project is licensed under the MIT License.
"""

# Salvar o conteúdo em um arquivo README.md
readme_path = "/mnt/data/README.md"
with open(readme_path, "w", encoding="utf-8") as file:
    file.write(readme_content)
