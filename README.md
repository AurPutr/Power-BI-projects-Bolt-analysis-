# Data-Driven Supplier Review Analysis

## Description
The goal of this project was to analyze supplier review data to identify reviewer outliers, select tickets for calibration with the supplier, and propose additional data points for a more accurate evaluation process. Using Power BI for interactive visualizations and data exploration, the task involved a systematic review of the **Total Support Quality Score** and detailed question-level responses to uncover patterns, anomalies, and opportunities for supplier performance improvement.

---

## Project Overview
The project covered the following key stages:

- **Outlier Identification**
  - Calculated the average score per review ticket and computed the standard deviation (STD) to identify reviews deviating significantly from the norm.
  - Determined potential outliers based on both statistical variance and review context.
  - Marked suggested outliers visually (dark green dots) for clarity in Power BI.

- **Ticket-Level Quality Analysis**
  - **Ticket 2:** Flagged for potential inaccurate data due to the absence of any negative responses.
  - **Ticket 10 & Ticket 9:** Noted for high negative ratings in *Relevant additional customer education* and *Expressed empathy appropriately*.
  - **Ticket 5:** Approximately 50% of reviewers gave negative ratings for *Friendly & human tone*.

- **Calibration Recommendation**
  - Selected **Ticket 2** (suspected inaccurate data) and **Ticket 5** (strong negative feedback in tone-related questions) for calibration with the supplier.

- **Additional Data & Actions**
  - Suggested further review of **Ticket 10** and **Ticket 9** to validate negative rating patterns.
  - Proposed gathering additional data points (e.g., reviewer profiles, context of interaction, ticket complexity) to enhance analysis accuracy.
  - Recommended actions beyond score collection, such as qualitative feedback review and reviewer calibration sessions.

---

## Technologies Used
- **Power BI** – for interactive dashboard creation and visual data exploration
- **DAX** – for calculated measures (average scores, STD calculations)
- **Custom KPI & Conditional Formatting Logic** – to highlight outliers and priority tickets visually

---

## Install
To view or interact with this project:
1. Open the Power BI `.pbix` file in **Power BI Desktop**.
2. Ensure source data (supplier review dataset) is placed in the correct directory or connected via Power BI parameters.

---

## Code / Analysis Logic
- Loaded supplier review dataset into Power BI
- Created calculated columns for:
  - **Average Score per Ticket**
  - **Standard Deviation**
  - **Z-score thresholding** for outlier detection
- Applied filters and slicers to explore review results dynamically by ticket and reviewer
- Designed visuals:
  - **Scatter plot** for outlier identification (dark green = potential outliers)
  - **Stacked bar charts** for negative response distribution by question
  - **KPI cards** for calibration ticket selection

---

## Run
Once the dashboard is loaded in Power BI:
- Use the **Outlier Detection** page to identify reviewers with extreme deviations
- Check the **Ticket Analysis** page to view negative response patterns by question
- Refer to the **Calibration Recommendation** section for suggested tickets to discuss with the supplier

---

## Visual Insights
The dashboard includes:
- **Reviewer Outlier Plot** – average score vs deviation with visual outlier markers
- **Negative Response Breakdown** – per question and per ticket
- **Calibration Priority View** – highlighting selected tickets (Ticket 2 & Ticket 5) with reasoning
- **Additional Review Suggestions** – Tickets 9 & 10 for further qualitative evaluation
