# Lead Qualification & Appointment Booking

An n8n automation workflow that handles the full lead qualification and 
discovery call booking pipeline for high-ticket service businesses.

---

## What This Workflow Does

1. **Lead Capture** — Triggers from a landing page lead trap
2. **Data Validation** — Guards against spam and invalid data
3. **Lead Routing** — Switch node routes leads based on qualification criteria
4. **AI Qualification** — Multiple AI Agents (GPT-4o-mini) assess and engage leads
5. **Google Sheets CRM** — Appends and updates lead data across sheets in real time
6. **Follow-up Sequences** — Sends automated follow-up emails via Gmail
7. **Cal.com Integration** — Three booking status webhooks handle:
   - Emergency/repair bookings
   - Tune-up bookings
   - Standard discovery call bookings
8. **Wait + Re-engage Logic** — Waits between touchpoints and re-engages 
   unbooked leads with AI-crafted messages

---

## Tech Stack
- **Automation:** n8n
- **AI:** OpenAI Chat Model / GPT-4o-mini
- **Scheduling:** Cal.com (webhooks)
- **CRM:** Google Sheets
- **Email:** Gmail
- **Logic:** JavaScript Code nodes, Switch, If
---

## Workflow Structure

- `lead trap from landing page` → validation → Switch → AI Agent routing
- 3 parallel Cal.com webhook flows for booking status updates
- AI Agents 1–8 handle different lead states and follow-up paths
- Google Sheets updated at every stage for full pipeline visibility
