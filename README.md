# 🧪 Manual Testing Project – CRM System (Quotation & Sales Management)

This repository contains a complete set of **manual testing deliverables** for a web-based **CRM system** used for quotation generation, inquiry handling, and sales tracking. It includes structured bug reports, categorized summaries, and a detailed breakdown of all issues identified during testing.

---

## 👤 About

**Name:** Shivam Patidar
**Background:** B.tech(Cse), Maulana Azad National Institute of Technology (MANIT), Bhopal
**Role on this Project:** Manual Tester**

I tested this CRM application end-to-end as a hands-on QA project to apply core manual testing concepts — test design, exploratory testing, defect logging, and defect lifecycle tracking — on a real, functioning application rather than a toy demo.

---

## 🔍 Domain

**CRM (Customer Relationship Management)**
Focused on **quotation generation**, **inquiry handling**, **sales tracking**, **follow-ups**, and **reporting modules**, across both the **User side** and **Admin side** of the application.

---

## 🎯 Responsibilities

- Designed and executed manual test cases covering functional, UI/UX, and input validation scenarios
- Performed both structured and exploratory testing across User and Admin modules
- Logged detailed, reproducible bug reports (steps to reproduce, expected vs actual result, severity/priority, screenshots)
- Identified and flagged duplicate defects to keep the bug backlog clean
- Verified fixes through retesting and tracked defects to closure
- Collaborated with the development team on defect resolution

---

## 📊 Testing Summary

### ✅ Total Bugs Reported: **88**

### 📂 Bug Categories

| Category                  | Count |
|---------------------------|-------|
| Search Functionality      | 35    |
| Input Validation Issues   | 15    |
| UI/UX Issues              | 10    |
| Form Submission Issues    | 10    |
| Indexing Issues           | 5     |
| Other Issues              | 13    |

### 📌 Status
- **Closed:** 88 / 88 (100%)

### 🎯 Priority Breakdown
- **High:** 50
- **Medium:** 30
- **Low:** 8

### 🔁 Duplicate Issues
- **2 identified and merged**
  _Example: "Alphabets allowed in numerical field until error on submission" was raised independently on both User and Admin sides._

---

## 📁 Sample Defects

| Defect ID | Title | Category | Priority | Status |
|-----------|-------|----------|----------|--------|
| #1  | Invalid password handling shows generic error instead of specific message | UI/UX Issues | High | Closed |
| #10 | Mobile number field accepts alphabetic characters without validation | Input Validation Issues | High | Closed |
| #25 | Uploaded image not visible after successful upload | UI/UX Issues | High | Closed |
| #28 | Invalid email format not detected; form submission still succeeds | Form Submission Issues | High | Closed |
| #61 | New record indexing skips the index of a deleted record | Indexing Issues | Medium | Closed |

> Full defect list with steps to reproduce, environment, and screenshots: [Bug_Report.md](./Bug_Report.md)
> Complete category-wise summary: [Summary.md](./Summary.md)

---

## 🧠 Key Bug Patterns & Insights

- **Search logic gaps:** Several modules returned results only on exact/full-value matches and failed on partial input (dates, IDs, names) — while other search fields over-matched on any substring, returning irrelevant results. This pointed to inconsistent search-query logic (likely inconsistent use of exact match vs. `LIKE`-style partial match) across modules.
- **Validation gaps:** Numeric fields (mobile number, amount, port number) accepted alphabetic and special characters at entry time, only failing at submission — indicating missing real-time/inline validation.
- **Indexing behavior:** Deleted record indices were not reused for new records, causing non-sequential numbering — a backend data-handling issue rather than a UI bug.

---

## 🧰 Tools Used

| Tool               | Purpose                        |
|--------------------|---------------------------------|
| Chrome, Edge       | Cross-browser manual testing   |
| Lightshot          | Screenshot capture for bug evidence |
| Jira               | Bug reporting and tracking     |
| Excel              | Test logging and cross-checks  |
| Markdown / GitHub  | Documentation                  |

---

## ✅ Modules Tested

- Customer Information Management
- Quotation Creation & Search
- Inquiry Tracking & Follow-ups
- Sales & Invoicing
- Form Validation & Submission
- User Access & Role Management
- Settings & Configuration
- Reporting

---

## 📄 Disclaimer

This repository is created for **educational and portfolio purposes**. No real user data is included; all screenshots and examples are from a test environment.

---

> 👨‍💻 **Author:** Shivam Patidar
> 🎓 **MANIT Bhopal**
> 🧪 **Role:** Manual Tester
> 🗂️ **Project Domain:** CRM – Quotation & Sales Management System
