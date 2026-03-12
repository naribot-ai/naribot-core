# NariBot System Architecture

This document outlines the technical design of NariBot, focusing on the abstraction between low-bandwidth user interfaces and high-intelligence AI backends.

## 🟢 High-Level Flow

The system is designed as a "headless" AI navigator. It decouples the communication channel from the reasoning engine.

1. **User Input:** Feature phone (USSD/IVR) or Smartphone (Chat).
2. **Channel Gateway:** A generic API layer that converts telecom protocols to JSON.
3. **Core Orchestrator (Cloud Run):** Validates the session and determines the intent.
4. **Intelligence Layer (Gemini):** Processes vernacular queries and matches against livelihood data.
5. **Persistence (Firebase):** Stores SHG profiles, session states, and progress markers.
6. **Response:** Sent back through the gateway in the user's native tongue.

## 🏗️ Technical Stack

* **Compute:** Google Cloud Run (Serverless, auto-scaling for pilot loads).
* **AI/LLM:** Gemini (Multimodal & Vernacular focus).
* **Database:** Cloud Firestore (NoSQL for flexible entrepreneur profiles).
* **Logic:** Python-based framework.

## 📡 Interface Abstraction

To remain DPI-aligned and gateway-agnostic, NariBot uses "Adapters":

| Interface | Method | Data Requirement |
| :--- | :--- | :--- |
| **USSD** | Menu-driven / Session-based | 0% (GSM signaling only) |
| **IVR** | Voice-to-Text -> LLM -> Text-to-Voice | 0% (Voice call) |
| **Chat** | Direct API interaction | Low-bandwidth (2G/3G friendly) |

## 🛡️ Privacy & Security

* **Identity:** PII is minimized at the gateway level.
* **Data Sovereignty:** All data is processed within regional cloud boundaries.
* **Safety:** Custom guardrail layers sit between the LLM and the user to ensure advice is accurate and safe.
