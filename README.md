# Concierge-AI
 a WhatsApp-first, LLM-powered, multilingual hospitality agent with autonomous workflows and future voice expansion.
# Concierge AI — Hospitality Agent System (Free SaaS Project)

> Automating hotel-guest communication using LLMs, WhatsApp, and no-cost tools — built for scale, plug-and-play, and real-world testing.

---

## 🚀 Overview

Concierge AI is a multilingual, LLM-powered conversational agent designed to transform hotel guest experiences. It runs on WhatsApp (for now), resolves common requests, routes issues to staff, offers upsells, and maintains memory across sessions — all while being built entirely with free or open-source tools for MVP launch.

---

## 🧠 Problem It Solves

Hotels struggle with:

* Repetitive guest queries
* Manual escalation workflows
* Lost upselling opportunities
* Language and timing barriers

**Concierge AI** solves this by acting as an autonomous AI concierge across WhatsApp and future voice/chat channels — creating a smart, branded communication layer between guests and hotel ops.

---

## 🧩 Key Features

* ✅ WhatsApp-first guest interface (via Twilio sandbox)
* 🌐 Multilingual NLP responses
* 🤖 GPT-3.5/4 powered responses + prompt engineering
* 🧠 Guest memory and intent understanding
* 🛎 Task routing (e.g. room service, maintenance)
* 💬 Staff dashboard with alert and chat log
* 💼 Hotel-specific onboarding + multi-tenant SaaS
* 📊 Admin analytics & CSAT capture

---

## 🏗 System Architecture

```
        Guest (WhatsApp)
              ↓
        Twilio WhatsApp API
              ↓
       Express.js + OpenAI API
      ↙               ↘
   Redis            Supabase
 (session)         (guest, chat)
      ↓                 ↓
 Translation     Staff Dashboard
  Engine        (Next.js on Vercel)
      ↓                 ↓
     n8n      ← Task routing & workflows
```

---

## 🔧 Tech Stack (Free Tiers Only)

| Layer            | Tech                        |
| ---------------- | --------------------------- |
| Frontend (Admin) | Next.js + Tailwind (Vercel) |
| Backend          | Node.js + Express (Render)  |
| LLM API          | OpenAI GPT-3.5 (free trial) |
| Memory Store     | Redis (Upstash)             |
| DB + Auth        | Supabase                    |
| NLP Translation  | LibreTranslate (API/self)   |
| Bot Automation   | n8n.io                      |
| Messaging        | Twilio WhatsApp Sandbox     |

---

## 📦 SaaS Features

* Tenant-based hotel account system (Supabase RLS)
* Plug-and-play onboarding wizard (1-click hotel setup)
* Editable FAQs and task triggers
* Chat quotas, billing plan logic, and support for multiple staff

---

## 🧪 MVP Development Timeline

### Week 1: Core Setup

* WhatsApp sandbox, GPT integration
* NLP intents, Redis sessions
* Translation middleware

### Week 2: Workflows & Memory

* n8n setup for alerting & tasks
* Supabase chat log DB schema

### Week 3: Admin Dashboard (React)

* Login, message log, mark task done
* Slack/Telegram alert integration

### Week 4: CSAT & Upsells

* Guest feedback flow
* GPT-based upsell suggestion template

### Week 5: Multi-Tenant SaaS

* Hotel sign-up, metadata config
* Staff invite + default flows

### Week 6: Testing + Pilot

* Run simulations with real hotel users
* Deploy via Vercel/Render

---

## 🧪 Real-World Testing Steps

1. Set up test hotel with dummy data
2. Add hotel profile to Supabase via admin panel
3. Start guest conversation → test task escalation
4. Try feedback and upsell flows
5. Monitor via dashboard

---

## 🔐 Privacy & Compliance (Basic)

* Guest ID anonymization
* Token-authenticated API routes
* Data deletion on request
* PII redaction for OpenAI calls

---

## 📈 Key Metrics

* Resolution rate without staff
* Average response time
* Upsell conversion rate
* Escalation rate
* Guest satisfaction (CSAT)

---

## ✨ Future Roadmap

* IVR/voice interface (Whisper + ElevenLabs)
* Hotel PMS integrations
* Self-hosted LLMs for privacy
* Mobile admin app
* Travel creator concierge mode (local guides)

---

## 🧰 Contributing

This project is open to contributions! Beginner-friendly issues will be labeled soon.

* `client/` → Next.js admin panel
* `server/` → Express.js API, memory, LLM, flows
* `n8n/` → Workflow definitions

---

## 👨‍💻 Author & Maintainer

**Piyush Takrani** — Second year CS undergrad & AI systems builder

Connect:

* [LinkedIn](https://linkedin.com/in/piyushtakrani2805)
* [GitHub](https://github.com/chotushikari)

---

## 🧾 License

MIT License

---

## 🙏 Acknowledgments

* OpenAI for GPT
* Twilio for WhatsApp API
* Supabase, Upstash, Vercel, and n8n
* All the early testers who helped shape Concierge AI
