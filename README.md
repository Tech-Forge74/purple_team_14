# PURPLE — Round 2 Submission

## 1. Team Name
bugged out



## 2. Problem Statement & Solution Description

**Problem Statement:**

Users struggle to track their spending on OTT platforms, cab services, and other subscriptions. Our solution is a smart website that analyzes uploaded bank statements, automatically detects transactions from services like Netflix, Rapido, and Namma Yatri, and provides a clear breakdown of expenses to help users manage their money better.

**Proposed Solution:**

We propose developing SubSentry – an AI-powered Hidden Subscription Finder that automatically detects recurring payments from bank statements, identifies forgotten subscriptions, calculates unnecessary spending, and helps users manage or cancel subscriptions before they lose more money.



## 3. Selected Features

Your prototype must prioritize the functional implementation of **two selected features**. Other features may be represented through static UI elements and do not require functional implementation.

### Feature 1: Smart Transaction Detection

 Upload bank statements in PDF/CSV format.

 Automatically detect OTT, Rapido, Namma Yatri, and other subscription-related transactions.

 Categorize transactions based on service type.


### Feature 2: Expense Analysis & Insights

 Calculate total spending on each platform.

 Display monthly expense breakdowns using charts.

 Identify recurring subscriptions and highlight unnecessary spending.



## 4. Setup & Running Instructions

### Prerequisites
Python 3.10+, Node.js 18+, and npm must be installed.

### Clone the Repository
```bash
git clone <repository-url>
cd hidden-subscription-finder
```

### Backend Setup
```bash
cd backend
python -m venv venv
```

Activate the virtual environment:

Windows:
```bash
venv\Scripts\activate
```

Install dependencies:
```bash
pip install fastapi uvicorn pymupdf pandas python-multipart pytesseract pillow
```

Start the backend:
```bash
uvicorn main:app --reload
```

### Frontend Setup

Open a new terminal:
```bash
cd frontend
npm install
npm run dev
```

Access the application at `http://localhost:5173`.

Backend API documentation is available at `http://127.0.0.1:8000/docs`.

---

## 5. Feature Demonstration

### Feature 1: Smart PDF Scanner

1. Launch the application and navigate to the PDF upload section.
2. Upload a bank statement in PDF format and initiate the extraction process.
3. Review the extracted transaction details, including transaction dates, descriptions, debit amounts, credit amounts, and balances.
4. Verify the extracted information and correct any inaccuracies if required.
5. Export the extracted transactions as a CSV file.

**Expected Outcome:** The system successfully extracts structured transaction data from bank statements, reducing manual data entry and making financial information easier to analyze.

### Feature 2: Subscription Detection Engine

1. Navigate to the subscription detection dashboard after extracting transactions.
2. Initiate the subscription detection process on the extracted transaction data.
3. Allow the system to analyze transaction frequency, merchant descriptions, payment amounts, and recurring patterns.
4. Review detected subscriptions along with their frequency, estimated renewal dates, and confidence scores.
5. Verify detected subscriptions and view estimated monthly and yearly subscription expenses.

**Expected Outcome:** The system automatically identifies recurring payments and potential hidden subscriptions, providing users with better visibility into their subscription expenses and helping them identify unnecessary recurring payments.




