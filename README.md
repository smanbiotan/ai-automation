# AI Automation Projects

A collection of AI automation projects and workflows I created using n8n, Make.com, Zapier, APIs, webhooks, and AI agents.

These projects focus on automating repetitive tasks, connecting different applications, and improving business processes.

## Tools & Technologies

- n8n
- Make.com
- Zapier
- APIs & Webhooks
- AI Agents & LLMs
- Email & CRM Automation
- Business Process Automation

## Featured Projects

### n8n (`n8n/`)

| Project | What it does |
|---|---|
| AI Lead Qualification Agent | Form leads are scored 1-10 by Gemini, logged to a data table, and routed: hot → owner alert with a drafted reply, warm → AI reply, cold → nurture email, low confidence → manual review |
| Docs Support Bot (RAG) | Upload company docs into a vector store; a public chat agent answers only from those docs, cites the source file, and emails a human when it can't answer |
| Daily AI News Brief | Every morning reads 5 AI news RSS feeds, keeps the last 24 hours, and Gemini writes an HTML newsletter that is emailed out |
| AI Resume Screener | Candidates upload a PDF resume; Gemini scores it 0-100 against the job description, saves the result, alerts the hiring manager for shortlisted candidates, and thanks every applicant |

### Make.com (`make.com/`)

| Project | What it does |
|---|---|
| AI Invoice & Receipt Processor | Forwarded invoice emails are read by AI (vendor, number, date, subtotal, tax, total, category), totals are checked, and each record is saved as "verified" or flagged "needs review" |
| AI Job Application Tracker | A job post sent to a webhook gets an AI fit score, a tailored resume summary and a cover letter opener, saved to a tracker with a 7-day follow-up date |
| Job Follow-up Reminders (daily) | Every morning finds applications due for follow-up and emails a ready-to-send follow-up message |
| E-commerce Order Ops | New orders deduct stock per item, trigger low-stock alerts, and send the customer an AI-written thank-you email with a product suggestion |

### Zapier (`zapier/`)

| Project | What it does |
|---|---|
| Client Onboarding Autopilot | A new client record triggers an AI welcome email via Gmail, a Google Calendar kickoff event, and marks the client "Onboarded" |
| AI Review Monitor | New reviews get AI sentiment and a drafted reply; negative reviews alert the owner, positive ones are saved as testimonials (Paths) |

## How to import

- **n8n:** Workflows → Import from File → pick the `.json`, then reconnect your own Gmail and Gemini credentials.
- **Make.com:** Create a new scenario → ⋯ menu → Import Blueprint → pick the `.blueprint.json`, then reconnect Gmail, the data store and the webhook/mailhook.
- **Zapier:** the `.json` files are each Zap's definition in Zapier's own format (ZDL), for reference. Zapier has no one-click import for single Zaps, so rebuild them from the steps shown.

Personal email addresses are replaced with `you@example.com`. Set your own before running.
