SignalBridge Project Intelligence

Overview

SignalBridge is a technology company managing multiple large client projects. Project information such as updates, risks, decisions, and changing requirements is spread across different teams and business systems.

This project proposes an AI system that analyzes project information, identifies important risks and signals, and prepares a situation brief for project leaders.

Problem

During the trial, the AI:

* Treated isolated comments as major risks.
* Missed connections between information from different teams.
* Used outdated information.
* Needed information from multiple business systems.
* Recommended actions without enough evidence.
* Required different AI capabilities for different tasks.

Proposed Solution

An evidence-based, multi-stage AI system:


                    ┌─────────────────────────┐
                    │    Business Systems     │
                    └─────────────────────────┘
                               │
                               ▼
                    ┌─────────────────────────┐
                    │ Information Collection  │
                    └─────────────────────────┘
                               │
                               ▼
                    ┌─────────────────────────┐
                    │ Context & Recency Check │
                    └─────────────────────────┘
                               │
                               ▼
                    ┌─────────────────────────┐
                    │    Signal Detection     │
                    └─────────────────────────┘
                               │
                               ▼
                    ┌─────────────────────────┐
                    │     Risk Assessment     │
                    └─────────────────────────┘
                               │
                               ▼
                    ┌─────────────────────────┐
                    │     Situation Brief     │
                    └─────────────────────────┘
                               │
                               ▼
                    ┌─────────────────────────┐
                    │      Human Review       │
                    └─────────────────────────┘
                               │
                               ▼
                    ┌─────────────────────────┐
                    │     Final Decision      │
                    └─────────────────────────┘


The system connects information from different teams, checks its context and recency, identifies signals, assesses risks using supporting evidence, and prepares a situation brief.

Human Review

AI recommendations should **not be acted upon without human review**.

The AI provides the analysis, evidence, and recommendation. The project leader reviews the information and makes the final decision.

Example

Development → Payment API may be delayed
QA → Testing depends on Payment API
Project Manager → Release depends on testing
                    ↓
          Potential Release Risk

The AI connects these related signals and identifies that a Payment API delay could affect the release schedule.

Conclusion

SignalBridge should use AI as a **decision-support system**, with evidence-based analysis and human review before consequential decisions.
