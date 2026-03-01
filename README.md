# Manufacturing Quality & Scrap Analysis – Monthly Overview

## Project Overview
This project analyzes monthly manufacturing quality performance using production and defect data from January 2023.

The goal is to identify high scrap areas, understand defect drivers, and support data-driven quality improvement decisions.

An interactive Tableau dashboard is used to visualize key metrics and trends.

## Business Context
Manufacturing quality teams need clear visibility into scrap rates by production line, shift, and defect category to prioritize improvement actions.

This project simulates a real-world quality reporting scenario commonly used in manufacturing environments.

## Tools & Technologies
- Tableau Public (dashboard visualization)
- Python (exploratory analysis)
- CSV-based manufacturing quality data

## Tableau Dashboard
Interactive dashboard:
https://public.tableau.com/app/profile/emre.bulut/viz/ManufacturingQualityScrapAnalysisMonthlyOverview/Dashboard2

## Key Insights
- Line 4 shows the highest scrap rate among all production lines.
- Fabric-related defects are the primary contributor to quality losses.
- Scrap rates are similar across Day and Night shifts.
- Line 4 is identified as a priority area for quality improvement.

## Project Structure
- `data/` – Dataset and data description
- `notebooks/` – Python analysis notebook
- `insights/` – Business findings and interpretations
- `tableau/` – Link to interactive Tableau dashboard

## Next Steps
- Automate monthly quality reporting
- Integrate AI-generated executive summaries
- Build an end-to-end reporting workflow using automation tools

## Automation & AI Use Case

### Conceptual Workflow

```
[Monthly Production Data]
        |
        | (CSV export from ERP / SharePoint)
        v
[Python Analysis Pipeline]
    - Load production quality data
    - Calculate scrap rate by line and shift
    - Dynamically identify worst-performing line
    - Identify top defect category
    - Generate executive summary text
        |
        v
[AI / Copilot Layer]
    - Refine summary into business-friendly language
    - Highlight key risks and focus areas
        |
        v
[Power Automate]
    - Triggered on monthly data refresh
    - Sends automated email to stakeholders
    - Includes:
        • AI-generated executive summary
        • Link to Tableau dashboard
        |
        v
[Decision Makers]
    - Review insights
    - Take corrective quality actions
```

This architecture demonstrates how manufacturing quality analytics can evolve from static reporting into an automation-ready, AI-enhanced decision support system suitable for enterprise environments.
