# Stock Trend Prediction App

A Streamlit web application for visualizing stock price trends and technical analysis using moving averages.

## 📊 Features

- **Interactive Stock Selection**: Enter any stock ticker symbol to analyze
- **Historical Data Analysis**: Displays stock data from 2010-2019
- **Statistical Summary**: Shows descriptive statistics of stock performance
- **Multiple Visualizations**:
  - Basic closing price chart
  - Closing price with 100-day moving average
  - Closing price with 100-day and 200-day moving averages
- **Technical Analysis**: Moving average crossovers for trend identification

## 🛠️ Technologies Used

- **Python 3.x**
- **Streamlit** - Web app framework
- **pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **pandas-datareader** - Financial data retrieval
- **Keras/TensorFlow** - Machine learning framework (for future predictions)

## 📋 Prerequisites

Make sure you have Python 3.7 or higher installed on your system.

## 🚀 Installation

1. **Clone the repository** (or download the script):
```bash
git clone <your-repository-url>
cd stock-trend-prediction
```

2. **Install required packages**:
```bash
pip install streamlit pandas numpy matplotlib pandas-datareader keras tensorflow
```

Or using requirements.txt:
```bash
pip install -r requirements.txt
```

## 💻 Usage

1. **Run the Streamlit app**:
```bash
streamlit run app.py
```

2. **Open your browser** and navigate to the local URL (typically `http://localhost:8501`)

3. **Enter a stock ticker** in the input field (e.g., AAPL, GOOGL, TSLA, MSFT)

4. **View the analysis**:
   - Statistical summary of the stock data
   - Closing price trends over time
   - Moving average analysis for trend identification

## 📈 Understanding the Charts

### Moving Averages Explained
- **100-day MA**: Short-term trend indicator
- **200-day MA**: Long-term trend indicator
- **Golden Cross**: When 100-day MA crosses above 200-day MA (bullish signal)
- **Death Cross**: When 100-day MA crosses below 200-day MA (bearish signal)

## 📁 Project Structure

```
stock-trend-prediction/
│
├── app.py                 # Main Streamlit application
├── README.md             # Project documentation
├── requirements.txt      # Python dependencies
└── models/              # Directory for ML models (if applicable)
```

## 📝 Requirements.txt

```txt
streamlit==1.28.0
pandas==2.0.3
numpy==1.24.3
matplotlib==3.7.2
pandas-datareader==0.10.0
keras==2.13.1
tensorflow==2.13.0
```

## 🔧 Configuration

- **Date Range**: Currently set to 2010-2019 (can be modified in the code)
- **Default Stock**: AAPL (Apple Inc.)
- **Data Source**: Yahoo Finance via pandas-datareader

## 🚨 Known Limitations

- Data is limited to 2010-2019 period
- Actual ML prediction functionality is not implemented in current version
- Requires stable internet connection for data fetching
- Some stock tickers may not be available through Yahoo Finance

## 🔮 Future Enhancements

- [ ] Implement actual stock price prediction using Keras model
- [ ] Add more technical indicators (RSI, MACD, Bollinger Bands)
- [ ] Extend date range to include recent data
- [ ] Add prediction accuracy metrics
- [ ] Include volume analysis
- [ ] Add comparison between multiple stocks

## 🐛 Troubleshooting

**Common Issues**:

1. **Import Error**: Make sure all required packages are installed
2. **Data Fetch Error**: Check internet connection and stock ticker validity
3. **Streamlit Not Opening**: Ensure port 8501 is available

**Error Solutions**:
```bash
# If pandas-datareader fails
pip install --upgrade pandas-datareader

# If matplotlib doesn't display
pip install --upgrade matplotlib

# Clear Streamlit cache
streamlit cache clear
```

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 Support

If you encounter any issues or have questions, please open an issue in the repository or contact [your-email@example.com].

---

**Note**: This application is for educational and informational purposes only. It should not be used as the sole basis for investment decisions. Always consult with financial professionals before making investment choices.
