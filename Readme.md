# 🤖 HirePilot — Autonomous AI HR Screening Agent

![n8n](https://img.shields.io/badge/Workflow-n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![LLM](https://img.shields.io/badge/LLM-Gemini%20%7C%20OpenAI-4285F4?style=for-the-badge)
![Automation](https://img.shields.io/badge/Type-AI%20Automation-00C7B7?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

**HireMind** is an intelligent, event-driven recruitment automation system built with n8n and LLMs that autonomously screens candidates, evaluates resumes, generates dynamic screening questions, computes ATS-style scores, and delivers personalized email feedback — all without manual HR intervention.

> Designed to simulate a real-world AI recruitment pipeline used in modern HR tech stacks.

---

![Workflow Overview](screenshots/workflow-overview.png)

---

## 🎯 Why This Project Matters

Traditional candidate screening is:

- ❌ Time-consuming  
- ❌ Manually intensive  
- ❌ Inconsistent across reviewers  
- ❌ Hard to scale  

**HireMind** solves this by introducing an AI-orchestrated workflow that standardizes and automates early-stage recruitment with production-style workflow engineering.

---

## ⚡ Core Capabilities

✅ AI-driven resume analysis  
✅ Dynamic screening question generation  
✅ Automated ATS compatibility scoring  
✅ Personalized candidate email responses  
✅ Fully event-driven workflow orchestration  
✅ Modular and extensible node architecture  
✅ Zero manual touch after form submission  

---

## 🏗️ System Architecture

### 🔄 End-to-End Pipeline



Candidate Form Submission
↓
Resume Extraction & Parsing
↓
LLM Semantic Analysis
↓
Dynamic Question Generation
↓
ATS Score Computation
↓
Automated Gmail Response


![Architecture Diagram](screenshots/architecture.png)

---

## 🧠 Workflow Deep Dive

### 1️⃣ Candidate Intake

- Triggered via form/webhook submission  
- Captures candidate metadata and resume  
- Normalizes incoming payload  

---

### 2️⃣ Resume Intelligence Layer

The workflow:

- Extracts structured data from resume  
- Identifies skills and experience signals  
- Prepares context for LLM evaluation  

**Goal:** Convert unstructured resumes into decision-ready data.

---

### 3️⃣ LLM Evaluation Engine

Using Gemini/OpenAI, the agent:

- Interprets candidate profile  
- Generates contextual screening questions  
- Assesses candidate relevance  
- Produces structured evaluation output  

**Design principle:** deterministic automation + probabilistic intelligence.

---

### 4️⃣ ATS Scoring Module

Custom scoring logic evaluates:

- Skill match  
- Experience relevance  
- Role alignment  
- Overall candidate strength  

Output is normalized into an ATS-style score for downstream decisions.

---

### 5️⃣ Automated Communication Layer

The system automatically:

- Generates personalized feedback  
- Sends Gmail response  
- Maintains professional tone  
- Closes the candidate loop  

**Result:** fully autonomous HR front-door.

---

## 📸 Workflow Preview

### 🧩 n8n Canvas

![n8n Workflow](n8n.png)

---


## 🛠 Tech Stack

| Layer | Technology |
|------|------------|
| Workflow Orchestration | n8n |
| LLM Engine | Gemini / OpenAI |
| Automation Logic | JavaScript (Code nodes) |
| Email Service | Gmail API |
| Data Processing | Structured JSON pipelines |

---

## 🚀 How to Run Locally

### 1️⃣ Install n8n

```bash
npm install -g n8n
n8n start


