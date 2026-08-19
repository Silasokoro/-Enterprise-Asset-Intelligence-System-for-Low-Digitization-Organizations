# Enterprise Asset Intelligence System for Low-Digitization Organizations

## Overview

Many organizations, particularly in developing economies, still rely heavily on Excel for managing critical operational data. While Enterprise Asset Management (EAM) platforms exist, they often require significant investment, dedicated IT support, and ongoing maintenance—making them impractical for many businesses.

This project demonstrates that organizations do not need expensive enterprise software to make intelligent asset management decisions.

The Enterprise Asset Intelligence System is a lightweight Python automation solution that transforms a standard Excel asset register into an intelligent decision-support system capable of automatically evaluating assets and recommending disposal actions based on maintenance economics.

Designed specifically for organizations that are not yet fully digitized, the solution runs locally on any authorized PC, requires no server infrastructure, no cloud subscription, and virtually no ongoing maintenance cost.

---

# Business Problem

Many organizations face several operational challenges:

- Asset records are managed entirely in Excel.
- Disposal decisions rely on manual judgment.
- Maintenance spending is rarely analyzed against acquisition costs.
- Asset reviews consume significant administrative time.
- Enterprise Asset Management software is often too expensive to acquire and maintain.

As a result, organizations continue investing in assets that are no longer economically viable.

---

# Solution

This project introduces a practical Business Intelligence solution that leverages Python to automate asset evaluation while preserving the organization's existing Excel-based workflow.

Instead of replacing familiar processes, the system enhances them with intelligent automation.

The application:

- Reads the organization's Excel asset register
- Cleans and validates maintenance data
- Calculates maintenance cost ratios
- Evaluates financial risk
- Generates disposal recommendations
- Creates an updated output worksheet
- Continuously monitors the Excel workbook for changes
- Automatically refreshes recommendations whenever new data is entered

Because everything runs locally, organizations gain automation without investing in costly digital infrastructure.

---
The Structure
Project Structure
Enterprise-Asset-Intelligence-System-for-Low-Digitization-Organizations/
│
├── README.md
│   └── Project overview, business problem, solution approach,
│       business value, technology stack, and implementation details
│
├── Enterprise_Asset_Intelligence_model.py
│   └── Main Python automation model
│       - Reads asset data
│       - Calculates maintenance ratios
│       - Generates asset risk scores
│       - Produces disposal recommendations
│       - Automates Excel output
│       - Monitors workbook updates
│
├── asset intelligence book.csv
│   └── Asset intelligence dataset used as project data
│
├── wokflow diagram.png
│   └── Visual representation of the Enterprise Asset Intelligence
│       workflow and decision-making process
│
├── requirements.txt
│   └── Python libraries required to run the model
│
└── .gitignore
    └── Specifies files and folders that should not be tracked by Git

# Why This Solution Matters

Digital transformation should not always begin with multimillion-dollar software implementations.

Many organizations simply need practical tools that improve operational decision-making while fitting within existing budgets.

This solution demonstrates how Python can extend Microsoft Excel into a lightweight decision intelligence platform that delivers measurable business value with almost no additional operating cost.

Benefits include:

- No cloud hosting costs
- No database server required
- No enterprise software licensing
- Minimal deployment complexity
- Easy adoption by Excel users
- Low maintenance requirements
- Immediate operational value

---

# Business Logic

Maintenance Ratio =

Lifetime Maintenance Cost ÷ Acquisition Cost

| Maintenance Ratio | Recommendation |
|-------------------|---------------|
| < 0.50 | Continue Use |
| 0.50 – 0.69 | Monitor Closely |
| ≥ 0.70 | Disposal Recommended |

The model automatically calculates a Financial Risk Score for every asset and classifies assets into actionable decision categories.

---

# Technology Stack

- Python
- Pandas
- OpenPyXL
- Watchdog
- Microsoft Excel

---
Enterprise-Asset-Disposal-Intelligence

│
├── data
│   ├── Asset_Intelligence_System.xlsx
│
├── notebooks
│   ├── Asset_Disposal_Analysis.ipynb
│
├── src
│   ├── asset_disposal_model.py
│
├── output
│   ├── Disposal_Model_Output.xlsx
│
├── images
│   ├── workflow.png
│   ├── dashboard.png
│
├── requirements.txt
│
├── README.md
│
└── LICENSE

# Business Value Delivered

The solution enables organizations to:

- Reduce manual asset reviews
- Improve disposal decision consistency
- Identify high-maintenance assets earlier
- Support evidence-based management decisions
- Lower operational costs
- Extend the value of existing Excel systems
- Begin digital transformation without expensive software investments

---

# Ideal Organizations

This solution is particularly suitable for:

- SMEs
- Manufacturing companies
- Educational institutions
- Facility management companies
- NGOs
- Logistics companies
- Security companies
- Organizations beginning their digital transformation journey

---

# Future Roadmap

Future enhancements include:

- Machine Learning asset failure prediction
- Remaining Useful Life (RUL) estimation
- SQL database integration
- Power BI dashboards
- Streamlit deployment
- Email notification engine
- API integrations
- Enterprise Asset Intelligence Platform

---

# Skills Demonstrated

- Business Intelligence
- Python Automation
- Operational Analytics
- Decision Intelligence
- Enterprise Asset Management
- Financial Risk Analytics
- Excel Automation
- Process Optimization
- Data Engineering
- Business Process Improvement

---
Disposal model updated successfully..

ASSET DISPOSAL RESULTS
          Asset Name  Maintenance Ratio (%)  Financial Risk Score Disposal Recommendation
      Perkins 100KVA                   81.0                  81.0    DISPOSAL RECOMMENDED
         LG Split AC                   67.0                  67.0         MONITOR CLOSELY
          CAT 150KVA                  106.0                 106.0    DISPOSAL RECOMMENDED
       Dell Latitude                   46.0                  46.0            CONTINUE USE
       Dell Latitude                   80.0                  80.0    DISPOSAL RECOMMENDED
         LG Split AC                   51.0                  51.0         MONITOR CLOSELY
     Lenovo ThinkPad                   71.0                  71.0    DISPOSAL RECOMMENDED
     Toyota Forklift                   38.0                  38.0            CONTINUE USE
Daikin Industrial AC                  108.0                 108.0    DISPOSAL RECOMMENDED
Daikin Industrial AC                   65.0                  65.0         MONITOR CLOSELY
        Toyota Hilux                   66.0                  66.0         MONITOR CLOSELY
       Dell Latitude                    6.0                   6.0            CONTINUE USE
      Toyota Corolla                   59.0                  59.0         MONITOR CLOSELY
        CAT Forklift                    6.0                   6.0            CONTINUE USE
        CAT Forklift                   54.0                  54.0         MONITOR CLOSELY
        HP EliteBook                   10.0                  10.0            CONTINUE USE
          CAT 150KVA                   41.0                  41.0            CONTINUE USE
      Perkins 100KVA                   67.0                  67.0         MONITOR CLOSELY
        HP EliteBook                   15.0                  15.0            CONTINUE USE
     Lenovo ThinkPad                   29.0                  29.0            CONTINUE USE
     Lenovo ThinkPad                   53.0                  53.0         MONITOR CLOSELY
          CAT 150KVA                   36.0                  36.0            CONTINUE USE
      Toyota Corolla                   45.0                  45.0            CONTINUE USE
        CAT Forklift                   21.0                  21.0            CONTINUE USE
      Toyota Corolla                   58.0                  58.0         MONITOR CLOSELY
        CAT Forklift                   58.0                  58.0         MONITOR CLOSELY
Daikin Industrial AC                   63.0                  63.0         MONITOR CLOSELY
         LG Split AC                   97.0                  97.0    DISPOSAL RECOMMENDED
        HP EliteBook                   63.0                  63.0         MONITOR CLOSELY
        HP EliteBook                   24.0                  24.0            CONTINUE USE
         Ford Ranger                   11.0                  11.0            CONTINUE USE
        Mikano 60KVA                   61.0                  61.0         MONITOR CLOSELY
     Toyota Forklift                   26.0                  26.0            CONTINUE USE
        HP EliteBook                   87.0                  87.0    DISPOSAL RECOMMENDED
Daikin Industrial AC                   89.0                  89.0    DISPOSAL RECOMMENDED
Daikin Industrial AC                   59.0                  59.0         MONITOR CLOSELY
        HP EliteBook                   90.0                  90.0    DISPOSAL RECOMMENDED
     Toyota Forklift                   54.0                  54.0         MONITOR CLOSELY
        Mikano 60KVA                   43.0                  43.0            CONTINUE USE
         Hyundai Bus                   91.0                  91.0    DISPOSAL RECOMMENDED
         Hyundai Bus                  102.0                 102.0    DISPOSAL RECOMMENDED
        Toyota Hilux                  101.0                 101.0    DISPOSAL RECOMMENDED
       Dell Latitude                   13.0                  13.0            CONTINUE USE
      Toyota Corolla                   99.0                  99.0    DISPOSAL RECOMMENDED
      Toyota Corolla                   93.0                  93.0    DISPOSAL RECOMMENDED
         LG Split AC                   23.0                  23.0            CONTINUE USE
         Ford Ranger                   30.0                  30.0            CONTINUE USE
         Hyundai Bus                   79.0                  79.0    DISPOSAL RECOMMENDED
      Toyota Corolla                   45.0                  45.0            CONTINUE USE
        HP EliteBook                   44.0                  44.0            CONTINUE USE

ASSET DISPOSAL SUMMARY
Disposal Recommendation
CONTINUE USE            20
DISPOSAL RECOMMENDED    15
MONITOR CLOSELY         15
Name: count, dtype: int64

Detected file update...

Reading updated asset master list...

Error: Bad CRC-32 for file 'xl/worksheets/sheet3.xml'

Developed by

Silas Okoro

Business Operations & Performance Data Scientist

Transforming everyday business processes into intelligent, low-cost decision systems using Python, SQL, Power BI and Data Analytics.


<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/5580a244-b4de-4dae-a331-1b7fe172e776" />

<img width="1356" height="469" alt="image" src="https://github.com/user-attachments/assets/8efededd-2dcd-4f67-9f44-f3211963b5e2" />

