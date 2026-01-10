# Talent View – HR Analytics

## Project Overview
This project analyzes HR data from the Talent View dataset to understand employee demographics, performance, attrition, and workforce trends using Power BI.

## Project Status
Work in Progress (Week 1)

## Work Completed
- Dataset downloaded
- Initial data understanding started

## Tools Used
- Power BI
- Excel / CSV
- GitHub
## Weekly Progress

### Week 1
- Collected and uploaded HR datasets
- Performed initial data understanding and cleaning
- Created data model in Power BI
- Built first dashboard page with core HR KPIs
- Added initial Power BI report and screenshots

## Week 2 Progress

- Completed Overview dashboard page with finalized KPIs
- Added Attrition and Retention metrics
- Improved visual layout and user-friendly slicers
- Uploaded updated Power BI report and dashboard screenshots


### Week 3 – Attrition Analysis (Completed)

- Built Attrition Analysis dashboard (Page 2)
- Attrition Rate & Retention Rate calculations
- Voluntary vs Involuntary attrition analysis
- Attrition by Department, Job Role, Gender
- Top attrition reasons (Top 3) with dynamic cards
- Attrition vs Avg Tenure analysis
- Conditional formatting & interactive slicers

### Week 4 – Hiring Analysis (Completed)

- Built Hiring Analysis dashboard (Page 3)
- New Hires KPI
- Hiring funnel: Applied → Screened → Interviewed → Hired
- Time-to-Hire analysis by Department
- Hiring distribution by Job Role
- Final Power BI report structure completed

- ---

##  Row-Level Security (RLS)

### Objective
To demonstrate an understanding of Row-Level Security (RLS) concepts in Power BI for HR analytics use cases.

---

### What is RLS?
Row-Level Security (RLS) restricts data access so users only see rows they are authorized to view.

In HR dashboards, RLS is commonly used to:
- Protect sensitive employee data
- Limit department-level visibility
- Ensure role-based access

---

### RLS Approach in This Project
This project is an **internship-level simulation**, so RLS is implemented conceptually based on available dataset fields.

| Role | Access Scope |
| Manager | Assigned department data |
| HR Business Partner (HRBP) | Department-level HR data |
| HR Director | Full organization data |


### Implementation Logic (Conceptual)
- RLS roles are created in **Power BI Desktop**
- Filters are applied using **Department / Job Level fields**
- Roles are tested using **“View as Role”**
- Final user-role assignment is done after publishing



### Example RLS Filter (Illustrative)
```DAX
[Department] = "Product_manager"


##  Data Refresh

- The dataset is sourced from local CSV files.
- Scheduled refresh is disabled in Power BI Service because local file paths are not accessible in the cloud.
- For production use, the data source can be migrated to:
  - OneDrive / SharePoint
  - Azure SQL Database
  - Data warehouse with on-premises gateway

Manual refresh was used during development.






