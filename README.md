# Potential Leads: AI-Driven Task & Inquiry Processor

An enterprise-grade automation suite built with **n8n** to ingest, fingerprint, and triage incoming business inquiries. The system features a deterministic de-duplication engine and an autonomous error-handling circuit to ensure 99.9% data integrity.

## 🛠️ System Architecture

The suite consists of two primary engines:

1.  **The Processor Core**: Ingests data via Webhooks and Gmail, generates a unique "Fingerprint" using JavaScript to prevent duplicates, and uses AI (OpenRouter) to dynamically assign priority and category.
2.  **The Sentinel (Error Handler)**: A specialized circuit that catches execution failures, updates the system state in Google Sheets to "FAILED," and alerts the administrator via Telegram.

## 🚀 Key Features

*   **Deterministic Fingerprinting**: Uses custom JS logic to create unique IDs based on task context, preventing redundant database entries.
*   **AI-Driven Triage**: Leverages LLMs to classify business impact (Priority) and operational domain (Category).
*   **Self-Healing State Management**: Automatically updates record status to reflect real-time processing success or failure.
*   **Instant Admin Alerting**: Real-time Telegram notifications with direct links to the failed execution logs.

## 👤 Developer
**Kariuki Mwangi**  
*AI Automation Engineer*  
