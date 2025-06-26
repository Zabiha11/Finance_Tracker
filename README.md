💰 Finance Tracker CLI App

A simple Python-based Command Line Interface (CLI) application that helps you track your income and expenses, view summary reports, and visualize spending trends using a CSV file.

📌 Features
✅ Add income or expense entries with date, amount, and description

📅 Filter transactions between any two dates

📊 View financial summaries (total income, expense, and net savings)

📈 Plot income vs expense graph over time

🗂️ Stores data in a local CSV file (finance_data.csv)

🗃️ Folder Structure

finance_tracker/
│
├── main.py               # Main CLI controller

├── data_entry.py         # Handles user input and validation

├── finance_data.csv      # CSV file storing all transactions

└── README.md             # Documentation

📦 Requirements

Python 3.7+

Libraries:

pandas

matplotlib

Install dependencies using:


pip install pandas matplotlib

▶️ How to Run

python main.py

📂 Options in CLI

Add a new Transaction

Prompts you to enter:

Date (or defaults to today)

Amount

Category: Income or Expense

Optional description

Saves it to finance_data.csv

View transactions and summary

Enter a start and end date

Displays transactions in the date range

Shows:

Total Income

Total Expense

Net Savings

Optionally, visualize data in a line chart

Exit

Safely exits the application

📈 Visualization
When viewing transactions, you can choose to plot a graph:

Green line for Income

Red line for Expense

This visual representation helps understand your cash flow over time.

📄 Sample CSV Data (auto-created on first run)

date,amount,category,description
26-06-2025,20000.0,Income,First stipend
26-06-2025,500.0,Expense,purchasing grocery
You can also add more sample data manually for testing.

⚙️ Functions Overview
main.py
main(): CLI interface

add(): Collects transaction input

CSV class: Handles CSV creation, insertion, and querying

plot_transactions(): Visualizes income vs expense trends

data_entry.py
get_date(): Validates date input

get_amount(): Ensures amount is valid

get_category(): Accepts 'I' or 'E' for Income/Expense

get_description(): Optional text input

🛠️ Customization Tips
You can change the CSV filename by modifying CSV_FILE in main.py.

Adjust graph frequency (daily/weekly/monthly) in the plot_transactions() function.

Extend the CLI menu with features like deleting or editing transactions.

👨‍💻 Author
Zabiha Muskan K
Student of Computer Science & Engineering | Passionate about Python, DSA, and AI

📝 License
This project is open-source and free to use under the MIT License.


