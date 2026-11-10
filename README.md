# Course Sales Performance Dashboard (Power BI)

An interactive Power BI dashboard analysing course sales by region and month, with row-level security so users only see the regions they are allowed to.

## What the Dashboard Shows
- **KPI cards:** Total Revenue (₹29,10,369), Total Orders (120), Total Customers (20)
- **Monthly Revenue Trend** line chart
- **Revenue by Region** bar chart
- **Course × Region matrix** with revenue and orders, colour-coded with conditional formatting
- **Slicers:** Year and Region

## Data Model
Star schema:

| Table | Role |
|---|---|
| `Fact_Orders` | Order transactions |
| `Dim_Customer` | Customer attributes |
| `Dim_Course` | Course catalogue |
| `Dim_Region` | Regions |
| `Dim_Date` | Date dimension |
| `Targets` | Revenue targets |
| `RLS_Map` | Maps users to regions for row-level security |

## Features
- Row-level security (RLS) by region
- Conditional formatting to highlight high and low performing courses
- Interactive year and region filtering

## Tools
Power BI Desktop · DAX · Power Query

## How to Use
Download the `.pbix` file and open it in Power BI Desktop.

## Repository Contents
```
├── README.md
├── screenshots/dashboard.png    # dashboard preview
└── model-files/                 # internal Power BI model parts
    ├── DataModel
    ├── DiagramLayout
    ├── Metadata
    ├── SecurityBindings
    ├── Settings
    ├── Version
    └── [Content_Types].xml
```
