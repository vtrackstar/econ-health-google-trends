# 📊 Economic & Health Trends Analysis

## 🧠 Overview
This project explores how public interest in fitness shifted between home and gym-based options during and after the COVID-19 pandemic. We blend **Google Trends** search data with economic indicators from **FRED (Federal Reserve Economic Data)** to reveal patterns in consumer behavior, fitness industry shifts, and broader economic sentiment.

---

## 📁 Data Sources

### Google Trends (U.S.-based keywords):
- **Home Equipment:** weights for home, yoga mat, resistance bands, adjustable dumbbell
- **Traditional Gyms:** gym membership, personal trainer, commercial gym
- **Gym vs Home Shift:** home workouts, gym near me
- **Group Fitness:** zoom fitness, HIIT class, spin class

### FRED (Economic indicators):
- **USREC:** Recession indicator (binary 1/0)
- **UNRATE:** Unemployment Rate
- **CPI:** Consumer Price Index (inflation)
- **UMCSENT:** University of Michigan Consumer Sentiment Index
- **PCE Services:** Personal consumption expenditures on recreation services
- **PCE Goods:** Personal consumption expenditures on recreation goods

## 🧰 Project Structure
├── notebooks/ # Jupyter notebooks with analysis & visuals

├── data/ # Raw input CSVs

├── README.md # Project overview and instructions

├── requirements.txt # Python dependencies

└── .gitignore # Ignore temp & env files

---

## ⚙️ Setup & Installation
1. Clone this repository:
git clone https://github.com/yourusername/econ-health-trends.git
cd econ-health-trends

2. (Optional) Create a virtual environment:

python -m venv env
source env/bin/activate   # Windows: env\Scripts\activate

3. Install dependencies:
pip install -r requirements.txt

4. Open and run the notebook:
jupyter notebook

---

### 🔍 Key Functions
load_fred_data(file_path): Reads & formats FRED data CSVs

clean_trends_data(file_path): Cleans and reshapes Google Trends data

reshape_trends(df, trend_label): Converts wide-format trends into long-format for analysis

pd.concat([...]): Combines all reshaped trend categories into a single DataFrame

### 📈 Next Steps
📊 Time series plots and moving averages of keyword trends

🧮 Correlation analysis between economic indicators and search behavior

🤖 Optional predictive modeling using economic variables to forecast fitness trends

📉 Regression or changepoint detection (e.g., impact of 2020 lockdowns)

📬 Contact

Feel free to connect or ask questions:

Bryan Louissaint

📧 balouissaint@gmail.com

📝 License

This project is licensed under the MIT License. Feel free to use, modify, and share with attribution.
