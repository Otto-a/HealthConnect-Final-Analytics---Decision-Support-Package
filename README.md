# HealthConnect Clinic Experience Lab — Data Analytics

**Programme:** AnalystLab Africa Experience Lab  
**Track:** Data Analytics  
**Pod:** HC-POD 4  
**Project:** Improving Patient Appointment Attendance Using Data and AI  
**Final Stage:** Week 8 (Final Integration, Presentation & Project Showcase)


## 📖 Project Overview
HealthConnect Clinic is an outpatient healthcare provider facing operational losses from missed appointments. 

Over 51% of scheduled appointments result in unannounced no-shows. This project analyzes 5,000 appointment records to uncover no-show patterns, validate communication channels, and deliver actionable operational rules to recover lost clinic capacity.



## 🚀 5-Week Project Journey (Weeks 4–8)

* **Week 4 (Kickoff & Problem Definition):** Audited the 5,000-record dataset. Verified logic integrity. Identified 4 key business questions and defined core KPIs.
* **Week 5 (Exploratory Data Analysis):** Imputed missing values with medians. Cleaned and separated cancelled visits. Discovered that SMS outperforms email and that no-shows book 10 days earlier on average.
* **Week 6 (Advanced Analytics & Integration):** Segmented lead times into 5 brackets. Discovered lead-time escalation (29.5% to 71.4%). Provided empirical cut-offs to the Data Science track.
* **Week 7 (Testing & Refinement):** Executed automated unit tests. Added baseline benchmark lines to visual charts. Validated alignment with the Data Science test set.
* **Week 8 (Final Integration & Presentation):** Packaged the final decision-support system. Finalized 4 clinic scheduling rules. Delivered executive slide deck and project video.



## 📊 Core Verified KPIs

| KPI Metric | Calculation | Verified Result | Business Meaning |
| :--- | :--- | :--- | :--- |
| **Baseline No-Show Rate** | $(2,423 / 4,737) \times 100$ | **51.15%** | Baseline clinic failure rate. |
| **Reminder Attendance Lift** | Reminded vs. Unreminded | **+4.78%** | Reminders increase overall attendance. |
| **SMS Performance Lift** | SMS vs. No Reminder | **+6.65%** | SMS is the single most effective channel. |
| **Critical Lead Time Exposure** | Bookings $>30$ Days | **48.40%** | Nearly half of appointments are in high-risk zones. |



## 💡 Key Validated Findings

1. **Lead Time Escalation:** Risk rises from **25.9%** (same-day) to **71.4%** (46–60 days). Risk crosses the clinic average after 30 days.
2. **Follow-Up Vulnerability:** Follow-up visits fail **62.1%** of the time with email, but drop to **49.1%** when sent via SMS.
3. **Compounding Prior History:** Patients with 2+ past missed visits fail at **62.1%**, and 4+ fail at **73.3%**.
4. **Senior Reliability:** Patients aged 65+ are the most reliable attending group (**48.07%** no-show rate).


## 📋 Actionable Clinic Scheduling Rules

* **Rule 1 (Two-Stage SMS Reminders):** Trigger SMS reminders at 7 days and 48 hours for bookings over 21 days old.
* **Rule 2 (SMS Mandate for Follow-Ups):** Route all follow-up appointment reminders exclusively through SMS.
* **Rule 3 (24-Hour Standby Pool):** Convert unconfirmed bookings over 30 days into a walk-in standby pool 24 hours prior.
* **Rule 4 (Chronic Offender Outreach):** Trigger direct front-desk phone calls for patients with 2 or more past no-shows.



## 🤝 Cross-Track Collaboration (HC-POD 4)

* **Data Science:** Provided empirical cut-offs (`lead_days > 30`, `past_no_shows >= 2`). Enabled model to achieve **99.8% recall** on long-lead visits.

