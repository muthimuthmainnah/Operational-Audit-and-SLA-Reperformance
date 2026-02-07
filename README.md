# Operational-Audit-and-SLA-Reperformance
# Operational Audit & SLA Reperformance

## 💡 Executive Summary

This project performed a comprehensive audit of customer support logs to validate data integrity and re-calculate operational metrics. The analysis moved beyond standard reporting to "reperform" business logic, verifying whether recorded Service Level Agreements (SLAs) aligned with actual timestamps.

The primary objective was to identify discrepancies in data recording and assess true operational performance against established benchmarks.

---

## 🔑 Key Findings

The audit uncovered critical insights regarding data quality and process alignment:

* **Data Integrity Issues:** Detected logical anomalies in a percentage of records, including "time travel" errors (resolution preceding response) and "ghost tickets" (closed status without resolution timestamps). *(Note: Update [Insert % based on your data] in your final text).*
* **SLA Compliance Gaps:** Recalculation revealed that **Critical Priority** tickets have a significantly higher breach rate than lower-priority tiers, indicating resource misalignment. *(Note: Update [Insert %] in your final text).*
* **Process Misalignment:** A discrepancy was identified between "Ticket Priority" and "Customer Sentiment," suggesting that current prioritization logic may not accurately reflect customer urgency.

---

## 🛠️ Methodology

This project focused on validating existing data through rigorous re-computation:

* **Data Integrity Validation:** Scanning logs for logical inconsistencies such as timestamps occurring out of chronological order or missing mandatory fields for closed tickets.
* **Business Logic Reperformance:** Ignoring pre-calculated SLA status fields and re-calculating actual response and resolution times based on raw start and end timestamps to determine true SLA compliance.
* **Metric Recalculation:** aggregating the re-performed data to evaluate breach rates across different priority tiers.

---

## 📂 Project Structure

* `audit_script.py` OR `audit_queries.sql`: The main script containing the logic for the audit and recalculations. *(Note: Replace with your actual filename depending on if you used Python or SQL).*
* `README.md`: This document providing an overview of the project findings.

---

## 🚀 How to Run the Analysis

To run the audit script locally:

1.  **Prerequisites:** Ensure you have the necessary environment set up (e.g., Python with Pandas, or a PostgreSQL interface like pgAdmin) depending on the script type.
2.  **Clone the repository:**
    ```bash
    git clone [Your Repository URL]
    ```
3.  **Data Setup:**
    * Ensure your source customer support logs data is available to the script (either imported into a database or placed as a CSV in the project directory).
4.  **Run the Script:**
    * Execute the main analysis script to perform the audit and view the recalculated metrics.

---

## 👤 Author

* **Muthmainnah** - https://www.notion.so/Muthmainnah-s-Portfolio-297641a84f1880869b42e875a69c3a6e?source=copy_link
