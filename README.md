# Stock Selection Tool

## Overview
The Stock Selection Tool is a Python application designed to help users analyze historical stock closing prices. It provides functionalities for user registration, login, stock data retrieval, analysis, and saving data for future reference.

---

## Features
- User registration and login system.
- Fetch historical stock data by ticker and date range.
- Perform analysis on stock closing prices, including:
  - Average price.
  - Percentage change.
  - Highest and lowest prices with the date
- Save analysis results to a CSV file.
- View saved data and trends.

---

## Prerequisites
Ensure you have the following installed:

- **Python**: Version 3.8 or later.
- **pip**: Python package installer.

### Required Libraries
Install the necessary libraries using pip:

```bash
pip install pandas yfinance
```

---

## Setup Instructions

1. Clone or download the repository:

```bash
git clone https://github.com/your-username/stock-selection-tool.git
cd stock-selection-tool
```

2. Verify that the following files are present in the project directory:
   - `main.py`
   - `functions.py`
   - `users.json` (optional, auto-generated during runtime if not present)

3. Ensure Python is installed and configured correctly on your system.

---

## Running the Application

1. Open a terminal or command prompt and navigate to the project directory.

2. Run the main script:

```bash
python main.py
```

3. Follow the on-screen prompts:
   - Register a new user or log in with an existing account.
   - Select options from the main menu to fetch stock data, view saved data, or analyze trends.

---

## Program Workflow

1. **User Registration/Login**: Provides secure user authentication using email and password.
2. **Fetch Stock Data**: Retrieve historical closing prices using the Yahoo Finance API by specifying a stock ticker and date range.
3. **Analysis**: Perform key analysis metrics like average price, percentage change, and high/low prices.
4. **Save and View Data**: Save analysis results to a CSV file and view them later as needed.

---

## File Descriptions

- **`main.py`**: The main script that manages user interactions and overall program workflow.
- **`functions.py`**: Contains reusable functions for user authentication, data fetching, analysis, and file handling.
- **`users.json`**: Stores user credentials in JSON format (auto-created during runtime).
- **`data.csv`**: Stores analyzed stock data (auto-created during runtime).

---

## Example Usage

### Fetch Stock Data Example
- Enter stock ticker (e.g., `AAPL`).
- Specify a date range (e.g., `2023-01-01` to `2023-03-01`).
- View analysis results, including average price and percentage change.
- Save the data to `data.csv` for future use.

### View Saved Data Example
- Select the "View Saved Data" option from the main menu.
- Display previously saved stock analysis data from `data.csv`.

---

## Additional Notes

- Ensure your system has an active internet connection for fetching stock data from the Yahoo Finance API.
- If no data is available for a specified stock ticker or date range, the application will notify you.
- Use valid email formats during registration to avoid errors.

---

## Troubleshooting

- **Missing Required Libraries**: Run `pip install pandas yfinance` to ensure dependencies are installed.
- **JSON Errors**: If `users.json` is missing or corrupted, delete the file and restart the application to auto-generate it.
- **CSV Save Errors**: Verify write permissions in the project directory.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.
