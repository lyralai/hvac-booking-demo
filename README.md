# 🔥 HVAC AI Booking Assistant

## What This Is
A 24/7 AI-powered booking assistant for HVAC and home services companies. It lives on a business's website as a chat widget, talks to customers, answers questions, captures leads, and books appointments directly into the business's calendar.

**Target market:** HVAC, plumbing, electrical, and other home services companies in the Vancouver, WA / Portland metro area.

**Business model:** $400/month per client. Cost to serve: ~$3/month per client. 99% gross margin. 13 clients = $5,200/month.

---

## Current Status

### ✅ Done
- **Interactive front-end demo** (`demo/index.html`) — a clickable mockup showing the full customer experience for a fictional HVAC company ("Cascade Heating & Cooling"). Demonstrates lead capture, appointment booking, FAQ handling, and a live stats dashboard. Hosted at: https://lyralai.github.io/hvac-booking-demo/

### 🔧 Next: Build the Real Working Version
The demo is a sales mockup — hardcoded responses, no real AI, no real calendar connection. To sign real clients, we need:

1. **Real AI conversation engine** — connect to OpenAI GPT-4o-mini or Claude API
2. **Google Calendar integration** — read available slots, create appointments
3. **Lead capture to CRM/sheet** — every conversation logged with name, phone, issue
4. **SMS confirmations** — Twilio integration for text reminders
5. **Embeddable chat widget** — drop-in script for any business website
6. **Per-client configuration** — business name, hours, services, pricing, calendar

**Tech stack for production:**
- n8n (automation/orchestration)
- OpenAI GPT-4o-mini (conversation)
- Google Calendar API (scheduling)
- Twilio (SMS)
- Vercel/Netlify (hosting, free tier)
- Vanilla JS or lightweight framework (chat widget)

---

## Unit Economics

| Item | Per Client/Month |
|------|-----------------|
| Revenue | $400 |
| LLM API (GPT-4o-mini) | $0.38 |
| Twilio SMS | $1.58 |
| Twilio phone number | $1.15 |
| Google Calendar API | $0 |
| **Total cost per client** | **~$3.11** |
| **Gross margin** | **~$397 (99%)** |

Fixed costs: ~$1/month (domain). n8n self-hosted = free.

| Clients | Monthly Revenue | Monthly Cost | Monthly Profit |
|---------|----------------|-------------|---------------|
| 1 | $400 | $4 | $396 |
| 5 | $2,000 | $16 | $1,984 |
| 10 | $4,000 | $32 | $3,968 |
| 13 | $5,200 | $41 | $5,159 |
| 15 | $6,000 | $47 | $5,953 |

Setup time per client: 1-2 hours. Maintenance: ~30 min/month per client.

---

## Repository Structure

```
├── README.md              ← you are here
├── demo/
│   └── index.html         ← interactive front-end mockup (live demo)
├── prompts/               ← system prompts for the AI conversation engine
│   └── MASTER_PROMPTS.md  ← lead scoring, email gen, follow-ups, LinkedIn, calls
├── n8n-workflow-template.json  ← drag-and-drop n8n workflow (import to n8n)
├── SETUP_GUIDE.md         ← 15-minute client onboarding guide
└── SALES_PAGE.md          ← product description / sales copy
```

---

## Goals

1. **Build the real working bot** (1-2 days) — replace mockup with live AI + calendar
2. **Get first client** — demo to a Vancouver/Portland HVAC company, free 14-day trial
3. **Reach 5 clients** ($2K/month) — validate the model
4. **Reach 13 clients** ($5K/month) — primary income floor

---

## Context

This project is part of a broader goal: build a recurring revenue business selling AI automation to local service companies. Starting with HVAC in the Vancouver/Portland market because:
- Strong local demand (aging housing stock, cold winters)
- HVAC companies have cash but no tech
- Every missed after-hours lead = $300-$5,000 lost revenue
- The ROI pitch is dead simple: "one saved job pays for the whole month"

---

## Owner
- **Alex D** ([@0xatd](https://github.com/0xatd) on GitHub)
- Vancouver, WA
