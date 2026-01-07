# fpa-copilot
AI-native FP&A Copilot that produces executive financial reads from messy, non-standardized income statements.
FP&A Copilot
What this is

FP&A Copilot is an AI-native decision support tool designed to replace the first financial read of a CFO or CEO.

The product takes messy, non-standardized income statements (DREs) — Excel, CSV, or raw exports — and produces a prioritized executive financial read, focused on what matters for decision-making speed and quality.

This is not a BI tool, ERP, or planning system.
It is a judgment layer, not a data infrastructure.

What this is NOT

FP&A Copilot explicitly does not aim to:

Replace ERPs or accounting systems

Build dashboards or financial statements

Perform full FP&A planning, budgeting, or forecasting

Require clean integrations (QuickBooks, NetSuite, SAP, etc.)

Enforce a fixed chart of accounts at this stage

If you are looking for:

Perfect data

Reconciled financials

Audit-grade outputs

This product is not for you.

Core Hypothesis

Even with imperfect data, an AI copilot can replace the first financial read of a CFO and materially improve decision-making speed and quality.

The product is built to test this hypothesis before investing in heavy normalization, integrations, or infrastructure.

MVP 0 — Decision Read
Objective

Validate whether decision-makers can trust and act on an AI-generated executive financial read without clean data.

Input

Messy, non-standardized DRE (Excel / CSV / text)

Inconsistent naming

Missing or partial line items

No enforced taxonomy

Output

A prioritized executive read, including:

Key financial KPIs

Major month-over-month movements

Outliers and anomalies

Explicit assumptions and caveats

Short qualitative insights focused on decisions, not reporting

What is intentionally missing

Normalized chart of accounts

Benchmarking

Forecasts

Dashboards

Long reports

Product Philosophy

Judgment > Presentation

Transparency > False precision

Speed > Perfection

Explicit uncertainty > Silent errors

If the model is unsure, it must say so.

Architecture (MVP 0)
User (Base44)
   → uploads DRE
n8n
   → file handling + orchestration
LLM (GPT)
   → financial interpretation + judgment
Base44
   → executive output


There is no database, no ERP sync, and no heavy backend logic at this stage.

Trust & Safety Principles

Every output must include:

Explicit assumptions

Known data gaps

Confidence indicators

“Nice but wrong” insights are worse than no insight.

The model must challenge the data, not blindly summarize it.

Roadmap Context (High-Level)

MVP 0: Decision Read (current)

MVP 1: Robust normalization with visible assumptions

MVP 2: Recurring reads (MoM / YoY)

MVP 3: Intelligent comparison without forced standardization

MVP 4: Executive narrative & critical questions

MVP 5: Signals & alerts with rationale

Only MVP 0 is in scope for now.

Status

🚧 Early MVP — under active development
This repository reflects experimentation, iteration, and hypothesis testing.
