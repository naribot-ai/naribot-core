# NariBot Core - API Overview

This document describes the logical interfaces used by NariBot Core. Actual deployments may vary based on telecom and AI providers.

## 1. Input Interface

### USSD / IVR Input
- User input via keypad (USSD) or speech (IVR)
- Normalized into structured query format

Example:
{
  "user_id": "session_id",
  "language": "kn",
  "input": "tailoring business",
  "channel": "ussd"
}

---

## 2. Orchestration Layer

Routes input to:
- Prompt engine (livelihood intelligence)
- Scheme discovery logic
- Decision flows

---

## 3. AI Interface

External LLM provider (e.g., Gemini)

Input:
- structured prompt
- context (language, geography)

Output:
- guided response
- next-step suggestions

---

## 4. Output Interface

Delivered via:
- USSD menu responses
- IVR voice output
- SMS fallback (optional)

---

## Notes
- API keys and production endpoints are not included
- Integrations depend on deployment environment
