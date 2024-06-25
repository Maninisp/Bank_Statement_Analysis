# Bank Statement Analysis

Welcome to the Bank Statement Analysis project. This repository provides tools to analyze bank statements using Python, supporting essential columns such as Date, Description, Amount, and Type. Whether you have real data or use generated statements, you can analyze transactions, calculate totals, track monthly trends, and identify extremes like maximum and minimum transactions. This tool is ideal for gaining comprehensive insights into your financial activities.

### Supported Columns
The analysis in this repository supports the following columns:
- **Date**
- **Description**
- **Amount**
- **Type**

### Generating Dummy Bank Statement
If you do not have an actual bank statement or statement with the above columns but still want to explore this repository, you can generate and analyze a dummy bank statement. The dummy bank statement data is generated in CSV and PDF formats using `generate_DummyStatement.ipynb`.

### Analysis Procedure
The analysis of the bank statement is performed in `analyse_statement.ipynb`.

## Files

### 1. `generate_DummyStatement.ipynb`

- **Purpose**: Generates a dummy bank statement in CSV and PDF formats.
- **Functionality**:
  - Creates transactions with random dates, descriptions, amounts, and transaction types.
  - Outputs data to a CSV file (`Bank_Statement.csv`).
  - Generates a PDF bank statement (`Bank_Statement.pdf`), as most banks provide statements in PDF format.

### 2. `analyse_statement.ipynb`

- **Purpose**: Analyzes the generated PDF bank statement.
- **Functionality**:
  1. **Convert Tables to Desired Format**:
     - Extracts tables from `Bank_Statement.pdf` and converts them into a structured format for analysis.
  2. **Total Sum of Debits and Credits**:
     - Calculates the total sum of debited and credited amounts.
  3. **Monthly Transaction Count**:
     - Counts the number of transactions done in each month.
  4. **Monthly Summary**:
     - Provides a summary of debits and credits for each month.
  5. **Max and Min Transactions**:
     - Identifies the maximum and minimum transaction amounts in the entire statement.
  6. **Visualize Monthly Credit and Debit Amounts**:
     - Visualizes the credit and debit amounts transacted in each month using a bar chart.

## Usage

### Generating Bank Statement:

- Open and execute `generate_DummyStatement.ipynb` to generate the dummy bank statement.
- Ensure necessary libraries (`fpdf`, `pandas`, etc.) are installed.

### Analyzing Bank Statement:

- Open and execute `analyse_statement.ipynb` to analyze the generated `Bank_Statement.pdf`.
- Install required libraries (`pdfplumber`, `pandas`, etc.) for PDF table extraction.
