# AI-Powered Open-Source Intelligence (OSINT) Footprint Analyzer

## 📌 Project Overview

The AI-Powered Open-Source Intelligence (OSINT) Footprint Analyzer is a cybersecurity-focused web application that helps users analyze their publicly available digital footprints and assess potential privacy risks. The system collects publicly accessible information from user-provided sources, evaluates exposure levels, calculates a risk score, and provides personalized recommendations to improve online privacy and security.

This project combines Artificial Intelligence, Machine Learning, and Open-Source Intelligence concepts to create an intelligent privacy assessment platform.

---

## 🎯 Problem Statement

Individuals unknowingly expose personal information through various online platforms such as public repositories, websites, professional profiles, and social networks. This information can be misused by attackers for phishing, identity theft, and cyber attacks.

Existing OSINT tools are often complex and expensive. This project aims to provide a simple and intelligent solution that analyzes digital footprints, identifies privacy exposure, and recommends security improvements.

---

## 🚀 Project Objectives

* Collect publicly available digital footprint information.
* Identify privacy exposure indicators.
* Calculate user privacy risk scores.
* Detect unusual exposure patterns using AI.
* Classify users into risk categories.
* Generate security recommendations.
* Visualize analysis results through dashboards.

---

## 🛠️ Technology Stack

### Frontend

* HTML
* CSS
* JavaScript
* Bootstrap

### Backend

* Python
* Flask

### Database

* SQLite

### Machine Learning

* Scikit-learn
* Isolation Forest Algorithm

### Data Processing

* Pandas
* NumPy

### APIs and Libraries

* GitHub API
* Requests
* BeautifulSoup

### Visualization

* Chart.js

---

## 📂 Project Modules

### Module 1: User Information Collection

* Accept user details
* Email address
* GitHub username
* Website URL

### Module 2: Digital Footprint Collection

* Retrieve public GitHub information
* Analyze website metadata
* Identify public exposure indicators

### Module 3: Exposure Detection

* Detect public emails
* Detect website exposure
* Analyze repository visibility

### Module 4: Risk Assessment

* Calculate privacy risk score
* Categorize risk level
* Generate exposure metrics

### Module 5: AI-Based Analysis

* Train Isolation Forest model
* Detect abnormal exposure patterns
* Predict privacy risk levels

### Module 6: Recommendation Engine

* Generate privacy recommendations
* Suggest security improvements
* Provide awareness messages

### Module 7: Dashboard and Reporting

* Risk score visualization
* Exposure analytics
* User recommendations

---

## 🗄️ Database Tables

### Users

* user_id
* name
* email
* github_username
* website_url
* created_at

### Footprint_Data

* footprint_id
* user_id
* github_found
* website_found
* public_email_found
* repository_count

### Risk_Assessment

* risk_id
* user_id
* risk_score
* risk_level
* analyzed_date

### Recommendations

* recommendation_id
* risk_id
* recommendation_text

### Analysis_History

* history_id
* user_id
* analysis_date
* result_summary

---

## 🤖 AI Algorithm Used

### Isolation Forest

Isolation Forest is an anomaly detection algorithm used to identify unusual digital exposure patterns. Users with excessive public information exposure are classified as higher-risk profiles.

---

## 📊 Expected Output

* Digital Footprint Analysis
* Privacy Risk Score
* Risk Classification (Low / Medium / High)
* Exposure Report
* Security Recommendations
* Interactive Dashboard

---

## 📅 Development Roadmap

### Phase 1

* Requirement Analysis
* Project Planning

### Phase 2

* UI Design and Development

### Phase 3

* Database Design

### Phase 4

* OSINT Data Collection Module

### Phase 5

* Risk Assessment Engine

### Phase 6

* AI Model Integration

### Phase 7

* Dashboard Development

### Phase 8

* Testing and Documentation

---

## 🔮 Future Enhancements

* Social Media Analysis
* Dark Web Exposure Detection
* Advanced Threat Intelligence
* Real-Time Monitoring
* Multi-Platform OSINT Integration

---

## 👩‍💻 Developed By

**Pradhicksha S**

Department of Artificial Intelligence and Data Science 

Mini Project 2026
