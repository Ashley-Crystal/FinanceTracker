# FinanceTracker

The Personal Finance Dashboard is a cross-platform web application designed to help individuals efficiently manage their finances, especially during life transitions such as moving to a new city. The app will provide features like tracking expenses, setting budgets, monitoring savings goals, and receiving weekly financial summary emails. The system will be integrated with trusted financial APIs to ensure accurate and real-time data processing.

Purpose and Goals :

The main objective of the Personal Finance Dashboard is to simplify financial management. It enables users to:

    Record daily transactions
    
    Create and track budgets across spending categories
    
    Get visual reports of their monthly expenses
    
    Receive automatic weekly emails summarizing their spending habits
    
    Monitor savings goals and calculate net worth over time
    
    Convert currencies when budgeting in a new country
    
    This tool is particularly useful for individuals relocating to a new city, where keeping control over spending is essential.


🚧 Phase 1 – Core Budgeting Features
Goal: Build a functional budgeting web app with Firefly III integration.

Tasks:

Set up a backend (Node.js/Express or Python/Flask) connecting to Firefly III:

Authenticate via OAuth2 or personal access token

Implement endpoints and UIs for:

Transaction management (view/create/edit/delete)

Budget creation and assignment per category

Monthly spending reports with category breakdown

UI in React or Vue:

Forms for entering transactions and budgets

Dashboard views with tables and charts

Outcomes:
A user can log expenses, set monthly budgets per category, and review summarized spending via a dashboard.

Phase 2 – Email Summaries Feature
Goal: Add scheduled weekly emails summarizing spending vs budget.

Tasks:

Use Firefly III API to fetch weekly transactions and summarize expenses per category.

Integrate Mailgun API:

Sign up (free tier: up to 100 emails/day, 1 domain) 
Use their REST API (or SMTP) to send HTML emails with summary charts/tables

Add backend scheduler (cron or node-cron):

Automatically run summary job weekly (e.g. every Sunday at 8pm)

Format data and send via authenticated Mailgun call

Outcomes:
Users get a weekly email with total spending, category breakdown, and budget alerts—keeping them on track.

Phase 3 – Net Worth & Savings Dashboard
Goal: Enhance the app by integrating YNAB for asset and savings tracking.

Tasks:

Add YNAB OAuth integration or personal access token

Fetch:

User’s budgets, account balances, and categories

Total assets vs liabilities and goal statuses

UI enhancements:

Net worth over time line chart

Savings goal tracking and projection

Combined dashboard view with Firefly and YNAB data

Outcomes:
Users can view their total financial health in one place—with budgets, spending, savings, and net worth visualized.

