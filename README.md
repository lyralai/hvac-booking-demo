# HVAC Lead Recovery Assistant

Interactive demo for selling a 24/7 AI booking and lead-recovery assistant to HVAC and home-service companies.

Live demo:
https://lyralai.github.io/hvac-booking-demo/

## What This Is

This repo contains a presentation-ready single-page product demo.

The demo shows three buyer-facing surfaces at once:

1. The HVAC company website a homeowner visits.
2. The AI booking conversation that qualifies and books the homeowner.
3. The owner dashboard showing the dispatch packet, workflow state, and recovered revenue estimate.

The current version is static HTML, CSS, and JavaScript. It is designed for a sales conversation, not production scheduling yet.

## Why An HVAC Company Should Care

HVAC owners lose money when web visitors and after-hours callers do not become booked jobs.

The pitch:

> We answer instantly, qualify the issue, capture contact and address, book the service window, and send the office a clean dispatch packet.

The simplest ROI story:

- A small repair can cover the monthly fee.
- A replacement quote can be worth thousands.
- After-hours leads are usually lost unless someone answers.
- Office staff should receive clean job summaries instead of vague chat transcripts.

## Demo Scenarios

The demo includes four scripted homeowner flows:

- No heat after hours
- AC leaking
- Maintenance tune-up
- Replacement quote

Each flow updates:

- lead count
- booking count
- estimated recovered revenue
- urgency
- customer details
- booking slot
- dispatch packet
- workflow checklist

## How To Run Locally

Open `index.html` in a browser.

Or serve it locally:

```bash
python3 -m http.server 4173
```

Then open:

```text
http://localhost:4173
```

## Current Product State

Implemented:

- Static interactive demo
- Responsive layout
- Homeowner website preview
- Booking chat simulation
- Scenario buttons for sales demos
- Lead qualification workflow
- Owner dashboard
- Dispatch packet view
- Estimated revenue recovery panel
- Presentation talk track in `PRESENTATION.md`

Not implemented yet:

- Real LLM conversation engine
- Real Google Calendar availability
- Real calendar booking
- Twilio SMS confirmation
- CRM or Google Sheets lead logging
- Per-client configuration
- Embeddable production widget script
- Authentication for owner dashboard

## Production Build Path

To turn this into a client-ready v1:

1. Add a small backend endpoint for chat messages.
2. Add per-client config: company name, hours, service area, phone, booking rules, emergency policy.
3. Connect Google Calendar to read availability and create appointments.
4. Log every lead to Google Sheets, Airtable, or a simple CRM table.
5. Send SMS confirmations and reminders through Twilio.
6. Package the customer-facing widget as one embeddable script.
7. Add an owner login with lead history and export.

Recommended first client offer:

> 14-day trial. We install the widget on your site, route leads to your existing calendar/phone workflow, and measure booked jobs recovered.

## Suggested Pricing

Simple local-services pricing:

- $399/month per location
- optional $499 setup fee
- 14-day trial for the first local proof customer

Keep the pitch tied to recovered booked jobs, not generic AI.

## Repository Structure

```text
index.html       Static interactive product demo
README.md        Product and repo overview
PRESENTATION.md  Sales talk track and demo script
```

## Owner

Repository accepted from `lyralai`.

Project operator:

- Alex / 0xatd
