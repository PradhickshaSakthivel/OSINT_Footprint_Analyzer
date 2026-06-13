# AI-Powered Open-Source Intelligence (OSINT) Footprint Analyzer

## 1. Approved Project Title

### Project Title

AI-Powered Open-Source Intelligence (OSINT) Footprint Analyzer

### Domain

Cybersecurity and Artificial Intelligence

### Technology Stack

* Frontend: HTML, CSS, JavaScript, Bootstrap
* Backend: Python Flask
* Database: SQLite
* AI/ML: Scikit-learn (Isolation Forest)
* Visualization: Chart.js
* APIs: GitHub API
* Libraries: Pandas, Requests, BeautifulSoup

---

## 2. Problem Statement

In today's digital world, individuals unknowingly expose personal information through various online platforms such as social media, public repositories, websites, and professional networking sites. This publicly available information can increase privacy risks and make users vulnerable to cyber threats, identity theft, and data misuse.

Existing OSINT tools are often complex, expensive, or designed for professional investigators. There is a need for a simple and intelligent system that can analyze publicly available digital footprints, assess privacy exposure levels, and provide recommendations for improving online security.

The proposed AI-Powered Open-Source Intelligence (OSINT) Footprint Analyzer aims to collect publicly available information, evaluate digital exposure, calculate privacy risk scores, and provide actionable recommendations using Artificial Intelligence techniques.

---

# 3. Project Objectives

### Primary Objective

To develop an AI-powered system that analyzes publicly available digital footprints and evaluates privacy exposure risks.

### Specific Objectives

1. To collect publicly available digital footprint information from user-provided sources.
2. To identify exposure indicators such as public emails, usernames, websites, and repositories.
3. To calculate a privacy risk score based on detected exposure factors.
4. To implement an AI-based anomaly detection model using Isolation Forest.
5. To classify users into Low, Medium, and High Risk categories.
6. To generate personalized security and privacy recommendations.
7. To provide an interactive dashboard for visualizing exposure and risk levels.
8. To maintain historical analysis records for future reference.

---

# 4. Module List

### Module 1: User Information Collection

* Accept user details
* Name
* Email
* GitHub Username
* Website URL

### Module 2: Digital Footprint Collector

* Collect publicly available information
* Retrieve GitHub profile details
* Analyze website metadata

### Module 3: Exposure Detection Engine

* Detect public email exposure
* Detect website exposure
* Detect repository visibility
* Identify exposure indicators

### Module 4: Risk Assessment Engine

* Calculate privacy risk score
* Categorize risk level
* Generate exposure metrics

### Module 5: AI-Based Anomaly Detection

* Train Isolation Forest model
* Detect unusual exposure patterns
* Predict risk severity

### Module 6: Recommendation Engine

* Generate security suggestions
* Recommend privacy improvements
* Provide awareness messages

### Module 7: Dashboard and Reporting

* Display risk score
* Display risk level
* Show charts and analytics
* Present recommendations

---

# 5. Use Case Diagram Submission

## Actors

### Primary Actor

User

### Secondary Actor

Administrator

## User Use Cases

* Register/Login
* Enter Profile Information
* Submit Footprint Analysis Request
* View Exposure Details
* View Risk Score
* View Recommendations
* View Analysis History

## Administrator Use Cases

* Manage Users
* View Reports
* Monitor System Usage
* Manage Dataset

## Use Case Diagram (Text Representation)

User
|
|-- Enter User Details
|-- Request Analysis
|-- View Risk Score
|-- View Exposure Report
|-- View Recommendations
|
Administrator
|
|-- Manage Users
|-- View Reports
|-- Monitor System

---

# 6. Table List

## Table 1: Users

| Field Name      | Data Type |
| --------------- | --------- |
| user_id         | INTEGER   |
| name            | TEXT      |
| email           | TEXT      |
| github_username | TEXT      |
| website_url     | TEXT      |
| created_at      | DATETIME  |

---

## Table 2: Footprint_Data

| Field Name         | Data Type |
| ------------------ | --------- |
| footprint_id       | INTEGER   |
| user_id            | INTEGER   |
| github_found       | BOOLEAN   |
| website_found      | BOOLEAN   |
| public_email_found | BOOLEAN   |
| repository_count   | INTEGER   |

---

## Table 3: Risk_Assessment

| Field Name    | Data Type |
| ------------- | --------- |
| risk_id       | INTEGER   |
| user_id       | INTEGER   |
| risk_score    | INTEGER   |
| risk_level    | TEXT      |
| analyzed_date | DATETIME  |

---

## Table 4: Recommendations

| Field Name          | Data Type |
| ------------------- | --------- |
| recommendation_id   | INTEGER   |
| risk_id             | INTEGER   |
| recommendation_text | TEXT      |

---

## Table 5: Analysis_History

| Field Name     | Data Type |
| -------------- | --------- |
| history_id     | INTEGER   |
| user_id        | INTEGER   |
| analysis_date  | DATETIME  |
| result_summary | TEXT      |

---

# 7. Database Schema Creation

## Objective

Design the database structure required for storing user information, digital footprint data, risk assessment results, and recommendations.

## Database Name

osint_analyzer.db

## Table 1: Users

| Column Name     | Data Type    | Description           |
| --------------- | ------------ | --------------------- |
| user_id         | INTEGER (PK) | Unique User ID        |
| name            | TEXT         | User Name             |
| email           | TEXT         | Email Address         |
| github_username | TEXT         | GitHub Username       |
| website_url     | TEXT         | Website URL           |
| created_at      | DATETIME     | Account Creation Date |

## Table 2: Footprint_Data

| Column Name        | Data Type    | Description               |
| ------------------ | ------------ | ------------------------- |
| footprint_id       | INTEGER (PK) | Unique Footprint ID       |
| user_id            | INTEGER (FK) | User Reference            |
| github_found       | BOOLEAN      | GitHub Profile Found      |
| website_found      | BOOLEAN      | Website Found             |
| public_email_found | BOOLEAN      | Public Email Found        |
| repository_count   | INTEGER      | Total Public Repositories |

## Table 3: Risk_Assessment

| Column Name   | Data Type    | Description     |
| ------------- | ------------ | --------------- |
| risk_id       | INTEGER (PK) | Risk Record ID  |
| user_id       | INTEGER (FK) | User Reference  |
| risk_score    | INTEGER      | Risk Score      |
| risk_level    | TEXT         | Low/Medium/High |
| analyzed_date | DATETIME     | Analysis Date   |

## Table 4: Recommendations

| Column Name         | Data Type    | Description            |
| ------------------- | ------------ | ---------------------- |
| recommendation_id   | INTEGER (PK) | Recommendation ID      |
| risk_id             | INTEGER (FK) | Risk Reference         |
| recommendation_text | TEXT         | Recommendation Message |

## Table 5: Analysis_History

| Column Name    | Data Type    | Description         |
| -------------- | ------------ | ------------------- |
| history_id     | INTEGER (PK) | History Record      |
| user_id        | INTEGER (FK) | User Reference      |
| analysis_date  | DATETIME     | Analysis Date       |
| result_summary | TEXT         | Summary of Analysis |

## Outcome

Database schema finalized and ready for implementation using SQLite.

---

# 8. UI Wireframe Design

## Objective

Create the initial wireframe design for the OSINT Footprint Analyzer.

## Screens Designed

### 1. Login Page

Components:

* Project Logo
* Email Field
* Password Field
* Login Button
* Register Link

### 2. Dashboard Page

Components:

* Navigation Menu
* User Profile Card
* Risk Score Card
* Exposure Summary
* Recommendation Section
* Analysis History

### 3. Analysis Form Page

Components:

* Name Input
* Email Input
* GitHub Username Input
* Website URL Input
* Analyze Button

### 4. Result Page

Components:

* Risk Score Meter
* Risk Level Indicator
* Exposure Details
* AI Recommendations
* Download Report Button

## Wireframe Tool Used

* Draw.io
* Figma
* Canva

## Outcome

Low-fidelity wireframes completed for all major project screens.

---

# 9. Login & Dashboard UI Design | Navigation & Form Design | Design Review | Frontend Environment Setup

## Login UI Design

### Features

* Responsive Design
* Email Input Field
* Password Input Field
* Login Button
* Forgot Password Link

### Technologies

* HTML
* CSS
* Bootstrap

---

## Dashboard UI Design

### Dashboard Components

#### Sidebar Navigation

* Dashboard
* Analyze Profile
* History
* Recommendations
* Logout

#### Main Dashboard

* User Summary
* Risk Score Card
* Exposure Count Card
* AI Analysis Card
* Recent Activities

---

## Navigation Design

### Navigation Menu Structure

Home
│
├── Dashboard
├── Analyze Profile
├── History
├── Reports
└── Logout

### Design Goals

* Easy Navigation
* Mobile Friendly
* Clean Interface

---

## Form Design

### User Input Form

Fields:

* Full Name
* Email Address
* GitHub Username
* Website URL

Button:

Analyze Footprint

### Validation

* Required Fields
* Email Validation
* URL Validation

---

## Design Review

### Review Checklist

| Component         | Status    |
| ----------------- | --------- |
| Login Page        | Completed |
| Dashboard Layout  | Completed |
| Navigation Menu   | Completed |
| User Form         | Completed |
| Responsive Design | Reviewed  |

### Improvements Identified

* Add Risk Meter Visualization
* Add Chart.js Dashboard Graphs
* Improve Mobile Responsiveness

---

## Frontend Environment Setup

### Software Installed

* Python 3.x
* VS Code
* Git

### Frontend Libraries

* Bootstrap 5
* Font Awesome
* Chart.js

### Project Folder Structure

OSINT-Footprint-Analyzer

├── static

│ ├── css

│ ├── js

│ └── images

├── templates

│ ├── login.html

│ ├── dashboard.html

│ ├── analysis.html

│ └── result.html

├── app.py

└── database

### Outcome

Frontend development environment successfully configured and ready for UI implementation.



