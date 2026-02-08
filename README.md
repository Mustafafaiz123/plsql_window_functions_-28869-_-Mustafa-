# plsql_window_functions_-28869-_-Mustafa-
**Business Context**

A private hospital operating within the Healthcare Services industry, specifically in the Medical Records and Billing Department.

**Data Challenge**

Patient records, doctor information, appointments, and billing data are stored in separate tables, making it difficult to analyze service utilization, patient activity, and revenue trends. Hospital management requires structured SQL analysis to improve operational and financial decision-making.

**Expected Outcome**

Generate insights such as the most consulted doctors, inactive patients, services with no appointments, billing trends over time, and patient segmentation based on billing amounts.

**3. Success Criteria (Exactly Five)**

Identify top 5 doctors by number of appointments → RANK()

Calculate running monthly billing totals → SUM() OVER()

Measure month-to-month billing changes → LAG()

Segment patients into quartiles based on total billing amount → NTILE(4)

Compute three-month moving averages of hospital revenue → AVG() OVER()
