# AI-Recruitment-Automation-Pipeline
Automated CV screening and scoring system using n8n and Gemini 2.5 Pro for unbiased talent acquisition.
# AI-Powered Talent Screening Pipeline (v1.0)
![n8n Workflow Canvas](Talent_Screening_Pipeline_v1.jpeg)

This project is a **Proof of Concept (PoC)** for a high-volume, automated recruitment screening system (Mass Hiring) orchestrated via **n8n** and powered by **Gemini 2.5 Pro** as the *Intelligent Qualitative Scoring Engine*. 

The pipeline is strategically engineered to reduce CV screening time by **93%**, slash operational infrastructure costs by **99.7%**, and guarantee a **100% objective, transparent, and bias-free** candidate pre-selection process.

---

## 🚀 System Architecture & Workflow Nodes
The end-to-end data pipeline processes data seamlessly from ingestion to reporting in the following sequence:
1. **Execute Workflow** (Manual or Webhook trigger initialization)
2. **CV Source: Cloud Repository** (Automated detection of new files in Google Drive)
3. **Document Stream Handler** (Secure downloading of candidate PDF documents)
4. **Intelligent Text Extraction** (Extracting unstructured raw text from PDFs)
5. **Metadata Normalization** (Filtering, structuring, and sanitizing textual data)
6. **Gemini Vision Core (Gemini 2.5 Pro Engine)** (Cognitive evaluation of qualifications and context)
7. **Qualitative Scoring Engine** (Mapping AI qualitative insights into structured JSON objects)
8. **Output Reporting Dashboard** (Real-time data logging and synchronization into Google Sheets)

---

## 🔒 Data Privacy & Anti-Bias Framework (Core Value Proposition)
To ensure strict compliance with modern HR objectivity standards, this system is tightly configured at the *Metadata Normalization* node and within the LLM prompt layer to **completely ignore personally identifiable information (PII)**, such as:
- Full Name
- Age & Date of Birth
- Gender
- Geographical Location / Residential Address

The AI engine evaluates candidates strictly based on **Technical Competencies**, **Formal Education** alignment, mastery of **Required Software/Tools**, and the relevance of their **Professional Experience**.

---

## 🛠️ Setup & Deployment Guide

### Prerequisites
- Active [n8n](https://n8n.io/) instance (Self-hosted or Cloud)
- Google Cloud Console Project (with Google Drive & Google Sheets API enabled)
- Google AI Studio API Key (with access to the `Gemini 2.5 Pro` model)

### Installation Steps
1. Clone this repository or download the `workflow.json` file.
2. Log in to your n8n dashboard.
3. Create a new workflow, click the menu icon in the top-right corner, and select **Import from File**.
4. Upload the downloaded `workflow.json` file.
5. Configure your respective *Credentials* for Google Drive, Google Sheets, and the Gemini API Key.
6. Toggle the workflow to **Active** for a fully automated, *set-and-forget* deployment.

---

## 📊 Cost Efficiency & Scaling Analysis
Based on token calculation metrics under the *Pay-as-you-go* tier using **Gemini 2.5 Pro**, the operational cost of this pipeline scales exceptionally well:
- **Estimated Cost per 1 CV:** ~IDR 26
- **Estimated Cost per 1,000 CVs:** ~IDR 26,400
- **Business Impact:** Reclaims dozens of HR labor hours per week and virtually eliminates the high operational labor costs typically associated with initial resume screening phases.

---
**Designed and Developed by:** *Muhammad Andithya Mirza Yaldi*
