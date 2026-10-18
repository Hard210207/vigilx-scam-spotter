# 🛡️ VigilX: ScamSpotter Core (SETU 2026 • PS-01)

**Developer:** Thakor Hard Jayprakash (Solo Participant)  
**Architecture:** IGOR-Inspired Deterministic Heuristic Core v1.0  

## ⚡ Overview
VigilX is a real-time, deterministic phishing and social-engineering detection web application built for **SETU 2026 (PS-01: Scam Spotter)**. Instead of relying on slow, black-box AI models that hallucinate false alarms, VigilX evaluates SMS, WhatsApp forwards, and live voice call transcripts in under 2 milliseconds using auditable regex and lexical state machines.

## 🔍 Core Capabilities
* **Visible Rule-Based Scoring (0–100):**
  * **Fake Urgency (+20):** Detects time-pressure triggers (`today`, `immediately`, `within 24 hours`, `tonight`).
  * **Account / Service Threat (+15):** Flags fear-inducing threats (`KYC is incomplete`, `account will be blocked`, `disconnected tonight`).
  * **Suspicious / Lookalike Links (+25):** Identifies non-official domains and insecure links (`.example`, `.xyz`, `.top`, `.click`, `http://`).
  * **OTP / Secret / Remote Access Extraction (+40):** Catches credential harvesting and screen-share lures (`share the OTP`, `share UPI PIN`, `install AnyDesk`).
* **False-Alarm Context Guard (0 pts):** Recognizes legitimate bank advisories (`NEVER share this OTP`, `Bank never asks`) to prevent false positives on genuine transactional messages.
* **In-Situ Highlighting & Explainability Matrix:** Color-codes exact trigger phrases inside the original message and provides a plain-language breakdown table.
* **AI Voice Call STT Guard:** Routes live microphone audio (via Web Speech API) or simulated call transcripts directly into the heuristic engine to detect "Digital Arrest" scams.
* **Actionable Remediation:** Provides risk-banded safety steps and direct access to India's National Cyber Crime Reporting Portal (`cybercrime.gov.in` / Helpline `1930`).

## 🚀 Quick Start
Zero build steps or external dependencies required.
1. Clone this repository.
2. Open `index.html` directly in any modern browser, or visit the live deployment link.
