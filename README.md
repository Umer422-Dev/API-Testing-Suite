# API-Testing-Suite
Manual REST API Test Cases and Bug Logging Report
# 🚀 REST API Testing & Bug Logging Suite

## 📌 Project Overview
This repository contains a comprehensive manual API testing suite and structured bug logging report. Testing was executed on RESTful API endpoints covering Authentication, Authorization, Product Management, and Office modules using **Scalar API Documentation/Client** interface with Bearer Token authorization.

---



## 📊 Test Execution Dashboard
* **Total Executed Test Cases:** 15
* **Passed Scenarios:** 9 (60%)
* **Failed Scenarios:** 6 (40%)
* **Total Bugs Identified:** 6 (3 High Severity, 3 Medium Severity)

---

## 🐛 Logged Bugs Summary

| Bug ID | Endpoint | Severity | Issue Summary | Status |
| :--- | :--- | :---: | :--- | :---: |
| **BUG-01** | `POST /api/Auth/register` | 🔴 HIGH | Weak password (`"123"`) accepted during registration | **OPEN** |
| **BUG-02** | `POST /api/Auth/login` | 🔴 HIGH | 500 Internal Server Error with stack trace on invalid password | **OPEN** |
| **BUG-03** | `POST /api/Product` | 🟡 MEDIUM | 500 Internal Server Error when Office ID does not exist | **OPEN** |
| **BUG-04** | `POST /api/Auth/login` | 🔴 HIGH | 500 Internal Server Error on non-existent username | **OPEN** |
| **BUG-05** | `GET /api/Product/{id}` | 🟡 MEDIUM | 500 Internal Server Error when Product ID does not exist | **OPEN** |
| **BUG-06** | `GET /api/Product` | 🟡 MEDIUM | Authentication Bypass (200 OK returned without Bearer Token) | **OPEN** |

---

## 📁 Project Deliverables
- 📄 **[Download Full QA Report (.xlsx)](./Michelin%20QA%20Report.xlsx)** — Complete test execution steps, expected vs actual results, and bug logging sheets.

---

## 🛠️ Tools & Technologies
- **API Documentation & Testing Interface:** Scalar UI (`localhost:5055/scalar/v1`)
- **Protocol:** HTTP / REST API
- **Authentication:** Bearer JWT Token
- **Format:** JSON Response Analysis
- **Documentation:** Microsoft Excel, GitHub Markdown
