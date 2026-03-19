# NariBot Core (α) 🚺💰
Navigating livelihood pathways for the next billion through vernacular AI and low-bandwidth channels.

NariBot is a Digital Public Infrastructure (DPI)-aligned, open-source AI system designed to bridge the economic divide for women job seekers and nano and micro-entrepreneurs. While most AI assistants require smartphones and high-speed data, NariBot delivers intelligence over missed call, IVR, USSD, and feature-phone-friendly interfaces.

---

## 🧩 The Challenge
In rural and peri-urban India, the "digital divide" is an interface problem. NariBot solves for:

- **Connectivity**: Works in zero-data environments (GSM/USSD signaling)  
- **Literacy**: Voice-first interaction (IVR) for non-text users  
- **Context**: Vernacular AI logic (Hindi, Marathi, Kannada, Tamil) grounded in local livelihood ecosystems  

---

## 🛠️ Tech Stack
We use a pro-code foundation to enable reliability and scale:

- **Intelligence**: Google Gemini *(external service; not part of open-source release)*  
- **Compute**: Cloud Run (Serverless)  
- **Data & Auth**: Firebase Ecosystem  
- **Interface Layer**: Telecom/voice gateway adapters (USSD, IVR, SMS)  

---

## 🏗️ Repository Scope
This repository acts as the **core orchestration layer ("brain")**, coordinating:

- Livelihood intelligence (prompt logic for job matching and scheme discovery)  
- Channel routing between USSD sessions and voice interactions  
- References to regional datasets and localized livelihood pathways  

> Note: Production infrastructure, API keys, and external service integrations are not included in this repository.

---

## 🚀 Use Cases

### 1. Livelihood Discovery
User explores viable business or job options based on location, language, and constraints.

### 2. Government Scheme Navigation
User identifies relevant schemes and receives guided next steps via voice or USSD.

---

## ⚙️ Quick Start 
This repository provides core orchestration logic and reference structures.

**To adapt:**
1. Clone the repository  
2. Configure your preferred telecom interface (USSD/IVR provider)  
3. Connect to an LLM provider (e.g., Gemini or equivalent)  
4. Localize prompts and datasets for your region  

---

## 🌍 SDG Alignment
NariBot contributes to:

- **SDG 1** - No Poverty  
- **SDG 5** - Gender Equality  
- **SDG 8** - Decent Work & Economic Growth  
- **SDG 9** - Industry, Innovation & Infrastructure  
- **SDG 10** - Reduced Inequalities  

---

## 🛡️ Responsible Use
NariBot is designed for inclusive and safe deployment:

- Minimizes data collection and avoids sensitive personal profiling  
- Provides guidance, not financial or legal guarantees  
- Designed to reduce exclusion due to language, literacy, or access barriers  

---

## 🚧 Status: Pilot Stage (Q1 2026)
Active pilot with 1,000+ entrepreneurs.

**Current focus**:  
- Hardening USSD menu-tree logic  
- Reducing voice latency  

---

## License
This project is licensed under the Apache 2.0 License. See the LICENSE file for details.

---

Built and maintained by BossMa Studio Works Pvt. Ltd. - Empowering livelihoods through accessible tech.
