[Uploading README_VNIT_Library.md…]()
# 📚 VNIT Library Usage & Resource Analytics Dashboard

## 🧭 Overview
An end-to-end analytics project for VNIT Nagpur's library using **Excel, Python, and Power BI**.
Analyzes borrowing trends, overdue patterns, book & author popularity, and student engagement to guide data-driven acquisition and policy decisions.

- Rows: 300 transactions (Dec 2024 - Mar 2025)
- Focus: **Usage Trends • Overdue & Fines • Book/Author Insights • Engagement**

## 🎯 Objectives
- Track monthly usage trends and department-wise borrowing.
- Identify most-borrowed books and authors for procurement planning.
- Reduce overdue rate via insights and reminders.
- Measure student engagement via feedback ratings.

## 🗂 Dataset
- File: `./Data/Library_Transactions.xlsx`
- Sheet: `Library_Transactions`

### Columns
Transaction_ID, Student_ID, Student_Department, Year_of_Study, Book_ID, Book_Title, Author_Name, Category,
Issue_Date, Return_Date, Days_Borrowed, Overdue_Days, Fine_Amount, Student_Rating, Issue_Mode, Library_Section

## 📊 KPIs
- **Total Books Issued** = COUNT(Transaction_ID)
- **Overdue %** = Overdue_Transactions / Total_Transactions × 100
- **Average Borrow Duration** = AVERAGE(Days_Borrowed)
- **Average Fine per User** = SUM(Fine_Amount) / DISTINCTCOUNT(Student_ID)
- **Avg Rating** = AVERAGE(Student_Rating)
- **Monthly Usage Trend** = SUM(Issues) by Month

See: `./Reports/Library_KPI_Summary.pdf`

## 📈 Dashboard (Corporate Blue)
1. Overview — Trend, Issues by Dept, Category split, Overdue %
2. Book & Author — Top titles & authors, Category breakdown, Rating vs Count
3. Department — Heatmap (Dept × Year), Fines & Overdues, Top Users
4. Engagement — Ratings trend, Fine distribution, Issue mode share

Layouts: `./Reports/Library_Dashboard_Layout_Plan.pdf`

## 📷 Screenshots
- `./PowerBI_Dashboard/Dashboard_Screenshots/Library_Overview_Page.png`
- `./PowerBI_Dashboard/Dashboard_Screenshots/Library_Books_Page.png`
- `./PowerBI_Dashboard/Dashboard_Screenshots/Library_Department_Page.png`
- `./PowerBI_Dashboard/Dashboard_Screenshots/Library_Engagement_Page.png`

## 📘 Reports
- KPI Summary — `./Reports/Library_KPI_Summary.pdf`
- Insights — `./Reports/Library_Insights_Report.pdf`
- Layout Plan — `./Reports/Library_Dashboard_Layout_Plan.pdf`

## 🧮 Tools
Python (Pandas, NumPy), Excel, Power BI

## 👨‍💻 Author
Bhaskar Maruti Sonawane  
B.Tech Metallurgical and Materials Engineering, VNIT Nagpur  
Email: bt22mme110@students.vnit.ac.in  
GitHub: https://github.com/BhaskarS7447

## 🪪 License
MIT
