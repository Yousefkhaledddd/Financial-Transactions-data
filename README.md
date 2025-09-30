🏦 Financial Transactions Analysis
This project executes an end-to-end data pipeline to analyze 13+ million financial transactions, providing insights into spending behavior, card usage, and customer demographics.

✨ Project Highlights
Database Integration: Designed and implemented a normalized schema in SQL Server for efficient data storage.

Big Data ETL: Used Python (Pandas, SQLAlchemy) for memory-efficient data joining and preprocessing via chunking.

Key Findings: Validated a strong income correlation among customers and identified the market dominance of Mastercard and Visa.

Interactive Reporting: Created a Power BI Dashboard to visualize trends and key metrics.

💾 Data & Schema
Table	Description	Example Columns
transactions	Records of card spending (Fact Table).	card_amount, use_chip
UsersData	Client demographics.	yearly_income, credit_score
CardsData	Card details.	card_brand, card_type

Export to Sheets
SQL Implementation
Data was loaded using a high-speed BULK INSERT into SQL Server, ensuring tables are linked by Foreign Keys (client_id, card_id).

🐍 ETL & Analysis
The Python pipeline connects to SQL Server, performs a LEFT JOIN to unify the data, and outputs a ready-for-analysis CSV file.

Key Analytical Findings:

Income Validation: A strong correlation was observed between Per Capita Income and Yearly Income.

Brand Share: Mastercard and Visa account for the vast majority of all transactions.

🖥️ Interactive Dashboard (Power BI)
The dashboard presents critical financial KPIs and trends:

KPI	Value
Total Transactions	13.3 Million
Total Amount	$571.84 Million

Export to Sheets
Visual Insights:

Channel Use: Online Transactions are the most frequent usage channel.

Transaction Trend: Annual volume stabilized around 1.39M transactions per year from 2016-2018.

🛠️ Tools & Technologies
Database: SQL Server

ETL/Analysis: Python (Pandas, SQLAlchemy)

Visualization: Power BI

🔗 Resources
Kaggle Dataset Source:
Financial Transactions Dataset
(https://www.kaggle.com/datasets/computingvictor/transactions-fraud-datasets/data)
