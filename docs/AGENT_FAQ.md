# AgentFlow Pro — Frequently Asked Questions

A comprehensive guide answering the most common questions from financial and insurance agents about how to use the automation workflows.

---

## Table of Contents

1. [General Questions](#general-questions)
2. [Getting Started](#getting-started)
3. [Lead Management (Workflows 01-02)](#lead-management)
4. [Policy & Renewal Management (Workflows 03, 09, 18)](#policy--renewal-management)
5. [Appointments & Scheduling (Workflow 04)](#appointments--scheduling)
6. [Commission & Income (Workflow 05)](#commission--income)
7. [Client Relationships (Workflows 06, 07, 08)](#client-relationships)
8. [Claims Support (Workflow 10)](#claims-support)
9. [Sales Growth (Workflows 11, 13, 20)](#sales-growth)
10. [Compliance (Workflow 12)](#compliance)
11. [Marketing & Outreach (Workflows 14, 15, 16)](#marketing--outreach)
12. [Professional Development (Workflow 17)](#professional-development)
13. [Market Intelligence (Workflow 19)](#market-intelligence)
14. [Troubleshooting](#troubleshooting)

---

## General Questions

### Q: What exactly is AgentFlow Pro?
**A:** AgentFlow Pro is a collection of 20 automation workflows that handle the repetitive, time-consuming parts of your daily sales activities. Think of it as a virtual assistant that never forgets a follow-up, never misses a renewal, and always has your daily briefing ready. Each workflow corresponds to a specific part of your job — lead management, follow-ups, renewals, appointments, commissions, compliance, and more.

### Q: Do I need to be technical to use this?
**A:** Not at all. The workflows are designed to run automatically based on schedules and triggers. You interact with them through simple forms (manual triggers) or they run on their own (scheduled triggers). If you can fill in a form with a client name and select a dropdown, you can use AgentFlow Pro.

### Q: Which workflows should I turn on first?
**A:** We recommend starting with these five core workflows, then expanding:
1. **Workflow 01** — Lead Capture & Routing (get leads organized)
2. **Workflow 02** — Client Follow-Up Sequences (never lose a lead)
3. **Workflow 03** — Policy Renewal Tracker (protect your book)
4. **Workflow 13** — Daily Sales Dashboard (know your numbers)
5. **Workflow 04** — Appointment Scheduling (stay organized)

Once comfortable, add Workflows 05 (commissions), 07 (birthdays), 08 (referrals), and 11 (cross-sell).

### Q: Can I customize the workflows for my specific practice?
**A:** Yes. Every workflow is fully customizable. You can adjust:
- Follow-up timing and frequency
- Email and SMS templates
- Lead scoring criteria
- Notification preferences
- Activity goals and benchmarks
- Reporting schedules

### Q: Will this replace my CRM?
**A:** No. AgentFlow Pro works alongside your existing CRM (Salesforce, HubSpot, AgencyBloc, Radiusbob, etc.). It automates the actions you'd normally do manually in your CRM — follow-ups, task creation, reminders, and reporting. Think of it as the automation layer on top of your CRM.

### Q: How does it connect to my existing tools?
**A:** AgentFlow Pro integrates through APIs and webhooks. It can connect to:
- Your CRM (for client data and activity logging)
- Your email platform (Gmail, Outlook, etc.)
- Your calendar (Google Calendar, Outlook Calendar)
- SMS providers (Twilio, etc.)
- Carrier portals (for rate and policy data)
- Social media platforms

---

## Getting Started

### Q: How do I activate a workflow?
**A:** There are two ways workflows run:
1. **Scheduled workflows** run automatically at set times (e.g., the renewal tracker runs daily at 7 AM). Just enable them and they work.
2. **Triggered workflows** run when something happens (e.g., a new lead comes in) or when you manually start them by clicking "Run workflow" and filling in the inputs.

### Q: How do I manually trigger a workflow?
**A:** Navigate to the Actions tab in your repository. Select the workflow you want to run. Click "Run workflow." Fill in the required fields (e.g., client name, action type) and click the green "Run workflow" button.

### Q: What are the "inputs" I see when running a workflow?
**A:** Inputs are the information the workflow needs from you. For example:
- The **Lead Capture** workflow asks for the lead's name, phone, email, and product interest
- The **Follow-Up** workflow asks which sequence type to start
- The **Quote** workflow asks for the client ID and product type

Each input has a description and many have default values, so you only need to fill in what's relevant.

### Q: How do I know a workflow ran successfully?
**A:** Each workflow run shows a green checkmark (success) or red X (failure) in the Actions tab. Click on any run to see the detailed logs and summary reports generated.

---

## Lead Management

### Q: How does the lead scoring work? (Workflow 01)
**A:** Each lead receives a score from 0-100 based on two factors:
- **Source quality:** Referrals score highest (30 points), followed by walk-ins (25), web forms (20), ad campaigns (15), and cold calls (5)
- **Product interest:** Higher-value products like investments and retirement (20 points) score higher than auto insurance (5 points)

A base score of 50 is given to all leads. Leads scoring 80+ are routed as "hot" to senior agents. Leads scoring 50-79 are "warm" and go to the standard queue. Below 50 goes to the nurture queue.

### Q: Can I change the lead scoring criteria?
**A:** Yes. Edit the scoring logic in Workflow 01 to match your priorities. For example, if your agency values health insurance leads more than auto, adjust the product scoring weights.

### Q: What follow-up sequences are available? (Workflow 02)
**A:** Five built-in sequences:
1. **New Lead** — 6-touch sequence over 30 days (welcome, call, email, call, email, nurture)
2. **Post-Meeting** — Summary email, proposal delivery, and follow-up
3. **Proposal Sent** — 5-touch sequence over 21 days to close the deal
4. **Policy Delivered** — Onboarding and satisfaction check
5. **Dormant Reactivation** — 3-touch sequence over 4 weeks to re-engage cold clients

### Q: What happens if a lead responds during a follow-up sequence?
**A:** When a lead responds (books an appointment, replies to email, etc.), you update their status in the CRM and the sequence advances or stops accordingly. For example, if they book a meeting after touch #2, the system moves them to the post-meeting sequence.

### Q: How quickly should I contact a new lead?
**A:** The workflow sends an automated acknowledgment within minutes. You should personally call within 24 hours. Studies show that contacting a lead within the first hour increases conversion by **7x** compared to waiting even two hours.

---

## Policy & Renewal Management

### Q: How does the renewal tracker alert me? (Workflow 03)
**A:** The tracker runs daily and creates alerts at four milestones:
- **90 days out:** Email campaign to client about upcoming renewal
- **60 days out:** Schedule a phone call to discuss renewal options
- **30 days out:** Urgent outreach with updated quotes
- **7 days out:** Critical — immediate call and escalation if no response

Each milestone has a different action plan and escalation level.

### Q: What if a client's policy lapses?
**A:** The workflow triggers the "expired policy" handler, which:
1. Notifies the client immediately about their coverage gap
2. Offers reinstatement options
3. Logs the lapse for compliance records
4. Adds the client to a re-engagement campaign
5. Alerts your manager if required by your agency

### Q: How does the multi-carrier quoting work? (Workflow 09)
**A:** When you request a quote:
1. The system pulls the client's profile and risk factors
2. Identifies which of your appointed carriers can write the policy
3. Submits quote requests to all eligible carriers
4. Compiles results into a side-by-side comparison chart
5. Adds your recommendation based on the client's needs
6. Packages everything into a professional PDF with cover letter

### Q: How does the client review scheduler work? (Workflow 18)
**A:** It automatically identifies clients due for review based on:
- **VIP clients:** Every 6 months
- **Standard clients:** Annually
- **Simple policies:** Every 18 months

It also triggers reviews when life events occur or when coverage gaps are detected. Before each review, it prepares a full package with coverage summary, gap analysis, and talking points.

---

## Appointments & Scheduling

### Q: What reminders do clients receive? (Workflow 04)
**A:** Clients receive:
- **24 hours before:** Email with meeting details, location/link, and documents to bring
- **1 hour before:** SMS text with quick-join link or address

You (the agent) receive a briefing with the client's history, products, and talking points.

### Q: How does the no-show handling work?
**A:** If a client doesn't show:
1. Wait 15 minutes, then call
2. If no answer, send a "we missed you" text
3. Send a reschedule email with your calendar link
4. The client's engagement score drops (-10 points)
5. A re-engagement task is auto-scheduled for 3 days later
6. If a second no-show occurs, it's flagged for manager review

### Q: Can clients self-schedule appointments?
**A:** Yes. The system generates calendar booking links that you can include in emails, texts, and your website. When a client books, the workflow handles confirmation, reminders, and your briefing prep automatically.

---

## Commission & Income

### Q: What does the commission tracker actually track? (Workflow 05)
**A:** Everything related to your income:
- **New policy commissions** (first-year and single-premium)
- **Renewal commissions** (trailing commissions on existing book)
- **Bonus qualifications** (quarterly, annual, carrier incentives)
- **Chargebacks** (monitors first-year policies for cancellation risk)
- **Income forecasting** (projects next 3 months based on pipeline and renewals)

### Q: How does chargeback monitoring work?
**A:** When you sell a policy, it enters a "chargeback window" (typically 12-13 months for life insurance). The system:
1. Tracks all policies in the chargeback window
2. Monitors for missed payments or cancellation signals
3. Triggers retention outreach if a policy is at risk
4. Alerts you before a chargeback hits so you can save the policy

### Q: Can I forecast my income?
**A:** Yes. The forecast workflow projects your income for the next 3 months based on:
- Policies in your current pipeline (weighted by close probability)
- Your existing renewal book
- Historical close rates and seasonal trends

---

## Client Relationships

### Q: What does the onboarding workflow do? (Workflow 06)
**A:** When a new client signs a policy, the system automatically:
1. Sends a welcome package (email + text) with your contact info, policy summary, and claims guide
2. Sets up the client in your CRM with proper tags and reminders
3. Creates a document folder and sends a collection request for any missing documents
4. Schedules check-ins at 30, 90, 180, and 365 days
5. Sets birthday and policy anniversary reminders

### Q: How does the birthday/anniversary outreach work? (Workflow 07)
**A:** The system checks daily for:
- **Birthdays:** Sends personalized email + text. VIP clients get a card or gift. Age milestones trigger product conversations (e.g., turning 65 triggers Medicare discussion).
- **Policy anniversaries:** Sends a thank-you with coverage review invitation. Multi-year milestones get special recognition.
- **Life events:** Marriage, new baby, new home, job change, retirement — each triggers specific outreach and product recommendations.

### Q: How does referral tracking work? (Workflow 08)
**A:** When you receive a referral:
1. Log it (referrer name + referred prospect)
2. Referrer gets an immediate thank-you (text, email, and later a handwritten card)
3. The referred prospect is created as a hot lead (highest priority score)
4. Contact within 24 hours with the referrer connection mentioned
5. If converted, the referrer is notified and receives their reward
6. Weekly report shows referral metrics, conversion rates, and top referrers

### Q: What referral rewards can I set up?
**A:** The system supports tiered rewards:
- **Tier 1** (1-2 referrals/year): Gift card
- **Tier 2** (3-5 referrals/year): Premium gift
- **Tier 3** (6+ referrals/year): VIP experience + policy discount

You define the specific rewards and the system tracks eligibility automatically.

---

## Claims Support

### Q: How does the claims workflow help me? (Workflow 10)
**A:** The claims workflow makes you the hero for your clients:
1. **Intake:** Guides you through collecting all required information and documents
2. **Filing:** Tracks submission to the carrier with claim number
3. **Follow-up:** Automatically follows up with adjusters on day 3, 7, 14, 21
4. **Client updates:** Sends status updates to your client at each milestone
5. **Escalation:** Flags claims with no progress for manager review at day 21+
6. **Post-claim:** After resolution, checks satisfaction and asks for referral

### Q: How often are open claims checked?
**A:** Every business day at 9 AM. The system checks all your open claims for status changes, overdue follow-ups, and approaching deadlines. You get a dashboard showing claims by status (new, in progress, awaiting adjuster, under review, settlement offered, closed).

---

## Sales Growth

### Q: How does cross-sell detection work? (Workflow 11)
**A:** Every Wednesday, the system scans your entire client book for:
- **Bundle opportunities:** Auto-only clients who could add home (and vice versa)
- **Coverage gaps:** Families without life insurance, professionals without disability
- **Upgrade needs:** Clients with insufficient coverage based on life changes
- **Product fit:** Age-based recommendations (retirement planning for 40+, Medicare for 65+)

Each opportunity comes with a recommendation card including talking points, estimated premium, and the best approach.

### Q: What does my daily dashboard show? (Workflow 13)
**A:**
- **Morning briefing (7 AM):** Today's appointments with client prep notes, priority follow-ups due, pipeline snapshot, renewals expiring soon, claims to check, and birthdays/events
- **End-of-day recap (6 PM):** Activity log (calls, emails, meetings, proposals, policies), progress vs. goals, wins, and carry-over tasks for tomorrow

### Q: How do I track my activity goals? (Workflow 20)
**A:** Default daily goals (customizable):
| Activity | Daily Goal | Weekly Goal |
|----------|-----------|-------------|
| Outbound Calls | 20 | 100 |
| Contacts Made | 8 | 40 |
| Appointments Set | 2 | 10 |
| Appointments Held | 2 | 8 |
| Proposals Sent | 1 | 5 |
| Applications | 1 | 3 |
| Referrals Asked | 2 | 10 |

The system tracks your actual numbers against these benchmarks and shows trend lines over 4 weeks with coaching insights.

---

## Compliance

### Q: What compliance items are tracked? (Workflow 12)
**A:** Four categories:
1. **Licenses:** All state licenses with expiration tracking (90/60/30-day alerts). If a license expires, sales are blocked and compliance is notified.
2. **Continuing Education:** Per-state CE hour requirements with progress tracking. Includes ethics-specific hours. Alerts if you're falling behind pace.
3. **E&O Insurance:** Errors & Omissions policy renewal tracking with coverage adequacy reviews.
4. **Disclosures:** Ensures all required disclosures (compensation, privacy, replacement, suitability) are documented for every transaction.

### Q: What happens if a license is about to expire?
**A:** Escalating alerts:
- **90 days:** Email reminder to begin renewal process
- **60 days:** Manager notification
- **30 days:** Urgent — must schedule renewal immediately
- **Expired:** All sales activity blocked + compliance team alerted

### Q: How does CE tracking work?
**A:** The system knows your state requirements (hours, categories, deadlines) and tracks your completed courses against them. It monitors your pace — if you should be 50% done at the midpoint and you're behind, it alerts you. It also tracks carrier-specific product certifications.

---

## Marketing & Outreach

### Q: What document collection is automated? (Workflow 14)
**A:** The system handles document requests for:
- **Applications:** ID, income proof, current coverage, signed forms
- **Claims:** Incident reports, photos, police reports, estimates, medical records
- **KYC/AML:** Multiple ID forms, proof of address, source of funds
- **Underwriting:** Medical exams, physician statements, driving records

Clients receive a secure upload link. If they don't submit by the due date, reminders escalate from friendly email (day 3) to phone call (day 7) to manager flag (day 14).

### Q: What email campaigns can I run? (Workflow 15)
**A:** Pre-built campaigns include:
- **Monthly newsletter** with market updates, tips, and referral reminders
- **Seasonal campaigns** (12 months of themed content)
- **Retention campaigns** targeting at-risk clients
- **Reactivation campaigns** for dormant clients
- **Product launch announcements**
- **Event invitations**

All campaigns track opens, clicks, unsubscribes, replies, appointments booked, and policies generated.

### Q: How does social media scheduling work? (Workflow 16)
**A:** Every Sunday, the system generates a weekly content plan:
- **Monday:** Educational tip
- **Tuesday:** Client success story
- **Wednesday:** Industry news
- **Thursday:** Personal brand / behind-the-scenes
- **Friday:** Fun fact or safety tip
- **Saturday:** Community involvement

Content suggestions are tailored per platform (LinkedIn = professional, Facebook = community, Instagram = visual). Analytics are tracked weekly.

---

## Professional Development

### Q: What certifications are tracked? (Workflow 17)
**A:** All major industry designations:
- CLU, ChFC, CFP, LUTCF, CPCU, CIC, CISR, RHU
- Carrier-specific product certifications
- Annual training requirements
- New product launch training

The system tracks status (active/in-progress/expired), renewal dates, and CE requirements for maintaining each designation.

---

## Market Intelligence

### Q: What does the rate monitor tell me? (Workflow 19)
**A:** Every Monday, you get:
- **Rate changes** from your appointed carriers (increases and decreases)
- **Impact analysis** showing how many of your clients are affected
- **Alternative carrier options** for clients facing increases
- **Re-quote opportunities** when competitors drop rates
- **Market intelligence** on regulatory changes, industry trends, and competitor activity

This lets you proactively reach out to affected clients before they find out on their own — positioning you as a trusted advisor.

---

## Troubleshooting

### Q: A workflow failed. What do I do?
**A:** Check the workflow run logs in the Actions tab. Common issues:
1. **Missing inputs:** Make sure all required fields are filled when manually triggering
2. **API connection:** Verify your CRM and email integrations are active
3. **Schedule issues:** Confirm the workflow is enabled (not disabled)

If a scheduled workflow fails, it will run again at the next scheduled time. You can also re-run it manually.

### Q: How do I change notification preferences?
**A:** Edit the notification settings in each workflow's environment variables. You can choose to receive alerts via:
- Email
- SMS/text
- Slack/Teams message
- Push notification
- Or any combination

### Q: Can I turn off a workflow temporarily?
**A:** Yes. In the Actions tab, select the workflow and click "Disable workflow." Re-enable it anytime. Your data and settings are preserved.

### Q: How do I add a new team member to the workflows?
**A:** Add them to the repository with appropriate permissions. Then update the routing rules in Workflow 01 and the notification settings to include their contact information.

### Q: What if I use a CRM that's not listed?
**A:** The workflows use standard API calls and webhooks that work with virtually any CRM. If your CRM has an API (most modern ones do), it can be connected. For CRMs without APIs, we support CSV import/export as a fallback.

### Q: Is my client data secure?
**A:** Yes. All data is:
- Encrypted in transit and at rest
- Stored in compliance with industry regulations
- Never shared with third parties
- Accessible only to authorized users
- Document uploads use secure, time-limited links

### Q: Can I use this on my phone?
**A:** Yes. The dashboards and reports are mobile-friendly. You can also trigger workflows and view summaries from the GitHub mobile app. Notifications can be sent as SMS for immediate mobile access.

---

## Still Have Questions?

Contact our support team or schedule a walkthrough session. We're agents too — we built this because we needed it ourselves.

*AgentFlow Pro — Automate the admin. Focus on the selling.*
