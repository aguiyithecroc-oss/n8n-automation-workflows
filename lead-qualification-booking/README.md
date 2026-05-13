# Lead Qualification & Appointment Booking

n8n workflow for qualifying leads and booking discovery calls automatically.
What This Workflow Does
Lead Capture — Triggers from a landing page lead trap
Data Validation — Guards against spam and invalid data
Lead Routing — Switch node routes leads based on qualification criteria
AI Qualification — Multiple AI Agents (GPT-4o-mini) assess and engage leads
Google Sheets CRM — Appends and updates lead data across sheets in real time
Follow-up Sequences — Sends automated follow-up emails via Gmail
Cal.com Integration — Three booking status webhooks handle:
Emergency/repair bookings
Tune-up bookings
Standard discovery call bookings
Wait + Re-engage Logic — Waits between touchpoints and re-engages unbooked leads with AI-crafted messages
Tech Stack
Automation: n8n
AI: OpenAI Chat Model / GPT-4o-mini
Scheduling: Cal.com (webhooks)
CRM: Google Sheets
Email: Gmail
Logic: JavaScript Code nodes, Switch, If
Workflow Structure
lead trap from landing page → validation → Switch → AI Agent routing
3 parallel Cal.com webhook flows for booking status updates
AI Agents 1–8 handle different lead states and follow-up paths
Google Sheets updated at every stage for full pipeline visibility
