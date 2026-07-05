# CrisisTrainer

CrisisTrainer is an AI-powered hospital crisis training and employee performance monitoring system developed to support staff preparedness during emergency and crisis situations.

The project integrates a web interface, FastAPI backend, structured JSON crisis knowledge records, RAG-based AI support, and a MySQL database to generate training scenarios, evaluate responses, and monitor performance.

# Project Overview

The purpose of this project is to provide hospital staff with realistic crisis training scenarios while enabling supervisors to assign tasks, monitor progress, and evaluate performance.

The system combines:

* AI-generated crisis training scenarios
* Employee dashboards
* Supervisor dashboards
* Role-based training tasks
* Database-based performance tracking
* AI-supported response evaluation
* Structured crisis knowledge records

---

# Features

## Employee Features

* User login
* Training participation
* Crisis scenario interaction
* Assessment question answering
* Performance tracking
* Employee dashboard

## Supervisor Features

* Supervisor dashboard
* Create crisis training scenarios
* Assign role-based training tasks
* Monitor employee activity
* View employee performance and feedback

## System Features

* Structured crisis datasets
* Multiple crisis categories
* Database integration
* Real-time monitoring interface
* AI-supported scenario generation
* Performance evaluation reports

---

# Technologies Used

## Frontend

* HTML5
* CSS3
* JavaScript

## Backend

* Python
* FastAPI
* SQLAlchemy

## Database

* MySQL
* phpMyAdmin

## Dataset

* JSON-based crisis scenario files
* Structured hospital crisis knowledge records

## AI Technologies

* OpenAI GPT API
* Retrieval-Augmented Generation (RAG)
* FAISS Vector Retrieval
* Structured crisis datasets
* JSON scenario files

---

# AI Integration

The system integrates OpenAI GPT models with structured crisis knowledge records to support crisis scenario generation, assessment question creation, response evaluation, and intelligent interaction within training activities.

The AI pipeline uses RAG and FAISS vector retrieval to retrieve relevant crisis knowledge and improve the quality of generated scenarios and feedback.

AI features may require an OpenAI API key during runtime configuration.

For security reasons, API keys are not included in this repository and should be provided locally by the user when running the system.

Example environment variable:

```text
OPENAI_API_KEY=your_api_key_here
```

The API key should never be uploaded to GitHub or shared publicly.

---

# Project Structure

```text
CrisisTrainer
│
├── ai-service/
│   ├── main.py
│   ├── database.py
│   ├── models.py
│   ├── schemas.py
│   ├── requirements.txt
│   └── crisis_trainer_full_pack/
│
├── crisis-trainer-frontend/
│   ├── css/
│   ├── js/
│   ├── login.html
│   ├── employee-dashboard.html
│   ├── supervisor-dashboard.html
│   └── live-monitor.html
│
├── database/
│   └── crisis_trainer.sql
│
└── README.md
```

---

# Installation Guide

## 1. Clone the repository

```bash
git clone https://github.com/CrisisTrainer-AI-Team/CrisisTrainer.git
```

Open the project folder.

---

## 2. Database Setup

Open phpMyAdmin and create a database named:

```text
crisis_trainer
```

Import:

```text
database/crisis_trainer.sql
```

---

## 3. Backend Setup

Navigate to:

```text
ai-service/
```

Create virtual environment:

```bash
python -m venv .venv
```

Activate environment:

```bash
.venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run backend:

```bash
python main.py
```

---

## 4. Frontend Setup

Open:

```text
crisis-trainer-frontend/login.html
```

Start using the system.

---

# Team Members

* Shahad Turki Alhoory
* Ghala Bander Alsuna Allah
* Hala Abdulmohsen Al-Shammari
* Jawaher Khalifah Al-Shammari
* Ghadah Mansour Al-Shammari

---

# Academic Purpose

This project was developed as an academic graduation project to support hospital crisis preparedness, staff training, and performance monitoring using artificial intelligence.

---

# License

Licensed under the MIT License.
