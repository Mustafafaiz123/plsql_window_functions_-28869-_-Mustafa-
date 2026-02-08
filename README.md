# plsql_window_functions_-28869-_-Mustafa-
**Business Context**

A private hospital operating within the Healthcare Services industry, specifically in the Medical Records and Billing Department.

**Data Challenge:**

Patient records, doctor information, appointments, and billing data are stored in separate tables, making it difficult to analyze service utilization, patient activity, and revenue trends. Hospital management requires structured SQL analysis to improve operational and financial decision-making.

**Expected Outcome:**

Generate insights such as the most consulted doctors, inactive patients, services with no appointments, billing trends over time, and patient segmentation based on billing amounts.


**3. Success Criteria (Exactly Five):**

Identify top 5 doctors by number of appointments → RANK()

Calculate running monthly billing totals → SUM() OVER()

Measure month-to-month billing changes → LAG()

Segment patients into quartiles based on total billing amount → NTILE(4)

Compute three-month moving averages of hospital revenue → AVG() OVER()

**Database Schema Design**

<img width="1075" height="711" alt="Screenshot 2026-02-08 022328" src="https://github.com/user-attachments/assets/8df75e9a-52fe-49b5-9323-5012a6717ca6" />



**5. SQL Scripts**
Table Creation

<img width="572" height="236" alt="Screenshot 2026-02-08 154348" src="https://github.com/user-attachments/assets/39a3d5d3-627f-4aed-bb47-a40a41e885eb" />

**6. Part A — SQL JOINs**
Retrieve valid patient appointments.
<img width="1066" height="210" alt="image" src="https://github.com/user-attachments/assets/9fda2573-5f43-4e07-b437-d4d338db505d" />

**2. LEFT JOIN**
Patients with no appointments.
<img width="892" height="225" alt="image" src="https://github.com/user-attachments/assets/ebd59c2e-6a22-415f-8ac9-c9d80ef13041" />

**3. RIGHT JOIN**
Doctors with no appointments.
<img width="846" height="242" alt="image" src="https://github.com/user-attachments/assets/58aa5fad-c21e-42b8-9f0b-9cecf789680f" />

**4. FULL OUTER JOIN**
Patients and doctors including unmatched records.
<img width="705" height="228" alt="image" src="https://github.com/user-attachments/assets/a23935e9-2afe-4537-bde7-9645ba52e307" />

**5. SELF JOIN**
Doctors within the same specialization.

<img width="913" height="250" alt="image" src="https://github.com/user-attachments/assets/fb79f53f-4e3e-4142-bdf5-b3ffcf5a155f" />

**7. Part B — Window Functions**
1. Ranking Functions
   
<img width="850" height="215" alt="image" src="https://github.com/user-attachments/assets/3d95c308-54f3-4724-9f94-b5026ecf9b64" />

**2. Aggregate Window Functions**
<img width="1066" height="215" alt="image" src="https://github.com/user-attachments/assets/08d4b852-44b2-4376-81af-0381f96b7cdb" />

**3. Navigation Functions**
<img width="1042" height="216" alt="image" src="https://github.com/user-attachments/assets/907b0987-80e6-40ba-b1c2-95dadd6c11ee" />

**4. Distribution Functions**
<img width="1038" height="228" alt="image" src="https://github.com/user-attachments/assets/5bcb30a2-33d3-4d83-a2a3-ce3349e93327" />

**8. Results Analysis**
**Descriptive**

Appointment frequency and billing amounts vary across doctors and patients.

Diagnostic

Variations are influenced by doctor specialization, patient demand, and service pricing.

Prescriptive

Hospital management should optimize doctor schedules, promote underutilized services, and focus on high-value patients.

**9. References**

Oracle SQL Language Reference

PostgreSQL Official Documentation

W3Schools SQL Tutorial

INSY 8311 Course Materials


