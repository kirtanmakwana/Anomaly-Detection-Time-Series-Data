---

# Anomaly Detection in Time Series Data

This repository provides an implementation of various anomaly detection techniques for time-series data using the **ADTK** (Anomaly Detection Tool Kit) library and Python.

---

## Features
- Load and preprocess time-series data from CSV files or Yahoo Finance.
- Apply multiple anomaly detection algorithms:
  - **Threshold Anomaly Detection**: Detects anomalies based on fixed thresholds.
  - **Quantile Anomaly Detection**: Identifies anomalies using percentile thresholds.
  - **Interquartile Range (IQR) Anomaly Detection**: Flags outliers based on statistical ranges.
  - **Generalized Extreme Studentized Deviate (ESD) Test**: Assumes normal distribution for anomaly detection.
  - **Persistence Anomaly Detection**: Detects anomalies based on significant changes compared to previous values.
  - **Volatility Shift Anomaly Detection**: Detects anomalies based on shifts in volatility over a defined window.

---

## Installation

### Prerequisites
- Python 3.8 or higher.
- Install required libraries using the command below:
  ```bash
  pip install -r requirements.txt
  ```
  *(Ensure the `requirements.txt` file lists dependencies like `adtk`, `pandas`, `matplotlib`, and `yfinance`.)*

---

## Usage

### 1. Clone the Repository
```bash
git clone https://github.com/kirtanmakwana/Anomaly-Detection-Time-Series-Data.git
cd Anomaly-Detection-Time-Series-Data
```

### 2. Prepare the Dataset
- Add a CSV file named `temperature.csv` with at least two columns:
  - `Date`: The date of observation.
  - `Mean`: The time-series data.
- Alternatively, use Yahoo Finance data by uncommenting relevant lines in the script.

### 3. Run the Script
Execute the `main.py` file:
```bash
python main.py
```

### 4. View the Results
- The script visualizes the anomalies detected using various methods. Each plot highlights anomalies in red.

---

## Examples

### Input
- **Dataset**: Time-series data from `temperature.csv` or stock prices from Yahoo Finance.
  
### Output
Visualizations showing anomalies detected by different algorithms.

---

## File Overview
- `main.py`: Main script implementing all anomaly detection methods.
- `temperature.csv`: Example dataset (user-provided).
- `requirements.txt`: List of required Python packages.

---

## References
- **ADTK Library Documentation**: [ADTK GitHub](https://github.com/arundo/adtk)
- **Yahoo Finance API**: [yfinance Documentation](https://pypi.org/project/yfinance/)

---

## Contributions
Feel free to submit issues or pull requests to improve this repository.

---

Let me know if you want additional customization or modifications for the README!
