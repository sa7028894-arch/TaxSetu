# TaxSetu



\*\*AI Autonomous Tax Compliance Platform for Micro-Enterprises\*\*



\## Overview

TaxSetu is a multi-agent AI system that automates GST/TDS tax compliance for micro and small enterprises. It ingests raw business transaction data, checks it against current tax rules, reconciles invoices, self-verifies its own calculations, and generates a plain-language compliance report — without requiring the business owner to have any tax expertise.



\\## Problem

Micro and small enterprises often lack the resources to navigate GST filings, TDS deductions, and input credit reconciliation. Manual bookkeeping and fragmented spreadsheets lead to missed deadlines, calculation errors, and lost input tax credit. Existing accounting software is typically too expensive, complex, or generic for businesses with no dedicated finance team.



\## Architecture



TaxSetu is built on a decentralized multi-agent pipeline:



\- \*\*Planner Agent\*\* — decomposes each compliance cycle (e.g. "file this quarter's GST return") into sequential milestones

\- \*\*Research Agent\*\* — gathers current tax rules, rate schedules, and filing deadlines

\- \*\*Domain Expert Agent\*\* — evaluates transaction data against regulatory requirements, flags mismatches and missing invoices

\- \*\*Execution Agent\*\* — reconciles invoices and calculates tax liability

\- \*\*Reviewer Agent\*\* — self-checks all calculations for consistency and compliance risk before anything reaches the business owner

\- \*\*Memory Manager\*\* — persists transaction history and prior filings across cycles

\- \*\*Report Generator\*\* — compiles everything into a clear, plain-language compliance report



\## Project Structure



TaxSetu/

├── agents/ # Agent definitions and orchestration logic

├── tools/ # Integrated utilities (tax rule lookup, reconciliation helpers)

├── output/ # Generated compliance reports

├── logs/ # Execution logs

├── main.py # Main orchestration pipeline

└── requirements.txt # Python dependencies





\## Tech Stack

\- \*\*Backend:\*\* Python, FastAPI

\- \*\*AI / Agents:\*\* Multi-agent orchestration with LLM-powered reasoning

\- \*\*Data:\*\* PostgreSQL for transaction storage, structured GST/TDS rule knowledge base

\- \*\*Deployment:\*\* Docker



\## Getting Started



\*\*Prerequisites:\*\* Python 3.10+



```bash

\# Clone the repo

git clone https://github.com/sa7028894-arch/TaxSetu.git

cd TaxSetu



\# Set up virtual environment

python -m venv venv

venv\\Scripts\\activate      # Windows

\# source venv/bin/activate # macOS/Linux



\# Install dependencies

pip install -r requirements.txt



\# Run the platform

python main.py

```



\## Status

Early development — core agent architecture and pipeline design in progress.

