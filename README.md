# Momo Data Analysis Dashboard

A comprehensive analytics dashboard for visualizing Mobile Money (MoMo) transaction data with filtering capabilities and detailed trancasction views.

## Features

- **Interactive Dashboard** with transaction type filtering.
- **Date Range** and **Amount Range** selectors.
- **Visualizations** of transaction volumes.
- **Detailed Transaction View** showing sender information and timestamps.
- **Monthly Transaction Summary** charts.

## How to Access
### Local Installation

1. Clone the repository

  git clone https://github.com/henryparfait/MoMo-Data-Analysis.git
 
2. Navigate to the project directory

cd MoMo_Data_Analysis

3. Open index.html in your browser

## How It Works
### Data Processing Pipeline

1. Extraction: Raw SMS data (sms.txt) is parsed by Extracting_Data.py

2. Cleaning: Cleaning_Data.py processes the extracted data

3. Storage: Structured data is saved to MTN.db SQLite database

4. Visualization: Front-end displays processed data with interactive filters

### Using The Dashboard
1. Filter Transactions:
- Select transaction types (Incoming Money, Payments to Code Holders, etc.)

- Set date range using the calendar pickers

- Adjust amount range sliders

2. View Visualisations: 
- Total transaction volume chart

- Monthly breakdown of transaction types

- Detailed transaction records with sender information
## Project Structure

MOMO_DATA_ANALYSIS/
├── Back-End/
│ ├── Cleaning_Data.py
│ ├── Database.py
│ ├── Extracting_Data.py
│ └── sms.txt # Raw SMS data input
├── Front-End/
│ ├── Assets/
│ │ └── logo.png # Dashboard logo
│ ├── index.html # Main dashboard page
│ ├── script.js 
│ └── style.css 
├── extracted_sms.txt 
├── structured_data.json
├── MTN.db 
├── schema.sql 
|---unmatched_sms.log
|---modified_sms_v2.xml
|---unprocessed_messages.txt
├── LICENSE
└── README.md

## Sample Transaction Data

The system processes SMS notifications in this format:

You have received 2000 RWF from Jane Smith (*******013) on your mobile money account at 2024-05-10 16:30:51. Message from sender: . Your new balance:2000 RWF. Financial Transaction Id: 76662021700.

## License

This project is licensed under the MIT License (https://opensource.org/license/mit)


