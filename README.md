TenderWise AI
 AI-Powered Tender Analysis & Bid Decision Support System

## Overview
TenderWise AI is an AI-powered tender analysis and decision-support platform designed to help organizations
evaluate tender opportunities more efficiently. Instead of manually reviewing lengthy tender documents and comparing
every requirement with a company's capabilities, TenderWise AI analyzes the tender and company profile, identifies
compliance gaps, evaluates risks, and generates a structured bid recommendation.
The system accepts two PDF documents: Tender Document and Company Profile. It then processes, analyzes, and
compares the information to generate a complete tender-readiness assessment.

## Key Features
1-Tender Document Analysis:
 • Tender title and category
 • Submission deadline
 • Eligibility requirements
 • Technical requirements
 • Financial requirements
 • Experience requirements
 • Required documents
 • Other tender-specific conditions 
2-Company Profile Analysis:
 • Company name
 • Services and capabilities
 • Experience
 • Certifications
 • Previous projects
 • Technical capabilities
 • Financial information
 • Registrations and relevant expertise
3-Requirement Matching:
 • Matched
 • Missing
 • Unclear
 • Supporting company evidence and explanations
4-Compliance Analysis:
 • Total requirements
 • Matched requirements
 • Missing requirements
 • Unclear requirements
 • Compliance percentage
5-Risk Analysis:
 • High Risk
 • Medium Risk
 • Low Risk
 • Risk description, potential impact, and supporting reason
6-Bid Decision Support:
 • BID
 • CONDITIONAL BID
 • NO-BID
 • Considers mandatory requirements, risks, and overall compliance
7-Submission Checklist:
 • Required documents
 • Missing mandatory requirements
 • Unclear mandatory requirements
 • Requirement priority
 • Recommended actions
8-AI-Generated Tender Report:
 • Executive Summary
 • Tender Overview
 •Company Overview
 • Compliance Summary
 • Matched Requirements
 • Missing Requirements
 • Unclear Requirements
 • Risk Analysis
 • Bid Recommendation
 • Key Reasons
 • Recommended Actions
 
## System Workflow:
Tender PDF
 +
Company Profile PDF
 ↓
Document Processing
 ↓
Tender & Company Analysis
 ↓
Requirement Matching
 ↓
Compliance Analysis
 ↓
Risk Analysis
 ↓
Bid Decision
 ↓
Report & Submission Checklist

## Project Architecture
TenderWise-AI/
■
■■■ .devcontainer/
■ ■■■ devcontainer.json
■■■ .streamlit/
■ ■■■ config.toml
■■■ assets/
■ ■■■ logo.png
■ ■■■ logo_icon.png
■■■ .gitignore
■■■ README.md
■■■ app.py
■■■ faizan_analysis.py
■■■ muteeba_matching.py
■■■ requirements.txt
■■■ sami_processor.py

## Core Modules
 app.py — Provides the Streamlit-based user interface and integrates the complete tender analysis pipeline.
 sami_processor.py — Handles PDF/document processing and prepares document information for the analysis
pipeline.
 faizan_analysis.py — Analyzes processed tender and company information and produces structured analysis results.
 muteeba_matching.py — Handles requirement matching, Matched/Missing/Unclear classification, compliance
 calculation, risk analysis, bid decision, AI-generated report, and submission checklist.

## Technology Stack
• Python
• Streamlit
• PyMuPDF
• OpenAI-compatible LLM API
• Google GenAI
• Pydantic
• Scikit-learn
• ReportLab
• python-dotenv

## Getting Started
1-Clone the repository:
 git clone https://github.com/Muteeba-pixel/TenderWise-AI.git
 cd TenderWise-AI
2-Install dependencies:
 python -m venv venv
 venv\Scripts\activate
 pip install -r requirements.txt
3-Configure Environment Variables:
 GROQ_API_KEY=your_api_key_here
Never commit API keys, passwords, or other sensitive credentials to GitHub. For Streamlit deployment, configure
sensitive credentials using Streamlit Secrets.
4-Run the Application:
streamlit run app.py

## Input
1-Tender Document: A PDF containing tender requirements, eligibility conditions, technical specifications, deadlines,
and submission requirements.
2-Company Profile: A PDF containing company information such as experience, services, certifications, projects,
financial information, and registrations.

## Output
• Tender overview
• Company overview
• Requirement matching
• Compliance percentage
• Missing requirements
• Unclear requirements
• Risk analysis
• Bid decision
• Decision reasoning
• Recommended actions
• Submission checklist
• AI-generated tender report

## Project Objective
The objective of TenderWise AI is to simplify and accelerate the tender evaluation process by transforming
unstructured tender and company documents into actionable business intelligence.
Can we apply?
What requirements do we already meet?
What are we missing or need to verify?
What should we do before submitting the bid?

## Team Project
TenderWise AI was developed as a collaborative project covering PDF processing and evidence handling, tender and
company analysis, requirement matching, compliance analysis, risk analysis, bid decision logic, report generation,
submission checklist, and Streamlit integration and user interface.

## Project Status
MVP — Functional
The current implementation includes the core tender analysis pipeline: PDF Upload → Document Processing →
Tender & Company Analysis → Requirement Matching → Compliance Analysis → Risk Analysis → Bid Decision →
Report & Checklist.

## Future Enhancements
• Tender deadline tracking
• Automated tender alerts
• Tender change notifications
• Interactive tender Q&A ;
• Proposal generation assistance
• Advanced evidence and page-level citations
• Historical tender comparison
• Multi-tender comparison
• Advanced analytics dashboard
• Enterprise-level authentication and access control

## Disclaimer
TenderWise AI provides AI-assisted analysis and decision support. The generated results may depend on the quality
and completeness of the uploaded documents. Users should verify important requirements, evidence, financial
information, legal conditions, and submission requirements before making an actual tender decision.

## License
This project is intended for educational, research, and demonstration purposes unless otherwise specified by the
project owners.
