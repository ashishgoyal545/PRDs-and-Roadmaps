# PRD: AI-Powered Feedback Summarizer

## 1. Context & Goal
Customer feedback is scattered across tickets, NPS verbatims, and app reviews. PMs spend hours consolidating themes.  
**Goal:** Auto-summarize top themes weekly with sentiment and impact.

## 2. Success Metrics
- -50% time to insights for PM/CS teams
- +25% coverage of feedback sources
- Counter: hallucination rate < 2% on benchmark set

## 3. Scope & Requirements
**User Stories**
- As a PM, I can connect sources (Zendesk, App Store, GSheets).
- As a PM, I receive weekly summaries with themes and sample quotes.
- As a PM, I can export a CSV of tagged feedback.

**Acceptance Criteria**
- OAuth flows, source toggles, weekly digest email.
- Theme clustering visible with counts & sentiments.

## 4. UX & Flows
Screens: Sources, Themes, Digest preview.

## 5. Data & Tech Notes
- Events: source_connected, theme_viewed, export_clicked
- LLM provider pluggable; caching for repeated prompts.

## 6. Rollout & Experiments
- Beta → GA after 8 design partner accounts
- A/B: digest vs dashboard-first

## 7. Open Questions
- PII redaction rules
- Multi-language support
