# risklens-cyberforge

# RiskLens

AI copilot that turns security alerts into ranked, explainable business-risk decisions.
Built by Team deepdefense for CyberForge by Mitigata.

## Problem
Security teams face alert overload, and technical severity does not show business risk.

## Solution
RiskLens deduplicates and correlates alerts into incidents, ranks them with an ML model,
maps them to MITRE ATT&CK, and uses an LLM to explain each incident and draft a playbook
from retrieved evidence only. A deterministic risk model estimates loss range and reporting
needs. Analysts approve, edit or reject every recommendation, and decisions are logged.

## Architecture
Alerts and logs -> dedup and correlation -> ML ranking -> MITRE mapping ->
LLM explanation -> risk model -> analyst approval -> audit log

## Tech stack (planned)
Python, pandas, scikit-learn, FastAPI, SQLite, Streamlit, LLM API,
MITRE ATT&CK, public datasets (UNSW-NB15 or CICIDS2017) plus synthetic alerts.

## Data and safety
Synthetic or public data only. No real systems are tested.

## Status
Idea stage. Prototype will be built during the hackathon.

## Team
MOHD AVAISH, Sartaj Ali
