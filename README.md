# AgentFlow Pro — Sales Automation Workflows for Financial & Insurance Agents

A comprehensive suite of **20 automation workflows** designed to streamline the daily sales activities of financial and insurance agents. From lead capture to policy renewal, from compliance tracking to commission forecasting — every workflow maps to a real activity in your sales day.

---

## Workflows

| # | Workflow | Trigger | Purpose |
|---|---------|---------|---------|
| 01 | Lead Capture & Routing | On new lead / Manual | Score, validate, and route incoming leads to the right queue |
| 02 | Client Follow-Up Sequences | On event / Manual | Automated follow-up cadences for every prospect stage |
| 03 | Policy Renewal Tracker | Daily 7 AM | 90/60/30/7-day renewal alerts and outreach |
| 04 | Appointment Scheduling | Hourly (business hours) | Book, confirm, remind, handle no-shows, prep agent briefings |
| 05 | Commission & Income Tracker | Weekly / On sale | Track commissions, chargebacks, bonuses, and forecast income |
| 06 | New Client Onboarding | On new client | Welcome kit, CRM setup, document collection, check-in schedule |
| 07 | Birthday & Anniversary Outreach | Daily 7 AM | Automated personal touchpoints and life-event product triggers |
| 08 | Referral Tracking | On referral / Weekly | Log referrals, thank referrers, track conversions, manage rewards |
| 09 | Quote Generation | On request | Multi-carrier quotes, comparison charts, professional delivery |
| 10 | Claims Support | Daily / On claim | Intake, carrier follow-up, client updates, post-claim satisfaction |
| 11 | Cross-Sell & Upsell Alerts | Weekly (Wed) | Scan client book for coverage gaps and revenue opportunities |
| 12 | Compliance Tracking | Daily 6 AM | Licenses, CE credits, E&O insurance, disclosure compliance |
| 13 | Daily Sales Dashboard | 7 AM & 6 PM | Morning briefing, EOD recap, weekly/monthly performance reviews |
| 14 | Document Collection | Daily / On request | Automated document requests, reminders, and tracking |
| 15 | Email & SMS Campaigns | Monthly / On demand | Newsletters, seasonal campaigns, retention, reactivation |
| 16 | Social Media Scheduler | Weekly (Sun) | Content planning, post scheduling, analytics review |
| 17 | Training & Certification | Monthly | Track designations, carrier certs, and professional development |
| 18 | Client Review Scheduler | Daily | Identify clients due for review, prepare review packages |
| 19 | Competitor & Rate Monitor | Weekly (Mon) | Carrier rate changes, market intelligence, impact analysis |
| 20 | Activity Log & Performance | Daily / Weekly | Track activities vs goals, conversion ratios, coaching insights |

---

## Project Structure

```
.github/workflows/          # All 20 automation workflow files
docs/
  SALES_PITCH.md            # Sales pitch document for presenting to agents/agencies
  AGENT_FAQ.md              # Comprehensive FAQ with answers on how to use each workflow
templates/                  # Email, SMS, and document templates (customizable)
scripts/                    # Helper scripts for data processing and integrations
```

---

## Getting Started

1. **Connect** your CRM, email, and calendar via API keys (stored as repository secrets)
2. **Configure** your preferences in each workflow's environment variables
3. **Enable** the workflows you want to activate in the Actions tab
4. **Run** — scheduled workflows start automatically; event-driven workflows trigger on activity

### Required Secrets

| Secret | Purpose |
|--------|---------|
| `CRM_API_URL` | Your CRM API endpoint |
| `CRM_API_KEY` | Your CRM API authentication key |
| `NOTIFICATION_WEBHOOK` | Slack/Teams webhook for notifications |

---

## Documentation

- [Sales Pitch](docs/SALES_PITCH.md) — Present AgentFlow Pro to agents and agencies
- [Agent FAQ](docs/AGENT_FAQ.md) — Answers to common questions about using the workflows

---

## Product Lines Supported

Life, Health, Property & Casualty, Auto, Home, Disability, Long-Term Care, Annuities, Investments, and Retirement Planning.

---

*AgentFlow Pro — Automate the admin. Focus on the selling.*
