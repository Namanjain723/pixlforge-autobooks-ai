<!-- PixlForge AutoBooks AI â€” README -->

<p align="center">
  <img src="assets/github_banner.png" alt="PixlForge AutoBooks AI" width="100%">
</p>

<h1 align="center">PixlForge AutoBooks AI</h1>
<p align="center"><b>An autonomous AI bookkeeping agent for US accounting & CPA firms.</b><br>
Reads invoices Â· writes weekly client reports Â· detects anomalies Â· onboards clients Â· tracks tax readiness â€” <b>24/7</b>.</p>

<p align="center">
  <img src="https://img.shields.io/badge/n8n-self--hosted-EA4B71?logo=n8n&logoColor=white">
  <img src="https://img.shields.io/badge/Claude_AI-Sonnet_4-D97757?logo=anthropic&logoColor=white">
  <img src="https://img.shields.io/badge/Python-3.11+-3776AB?logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?logo=streamlit&logoColor=white">
  <img src="https://img.shields.io/badge/Plotly-Charts-3F4F75?logo=plotly&logoColor=white">
  <img src="https://img.shields.io/badge/ReportLab-PDF-00897B">
  <img src="https://img.shields.io/badge/License-Portfolio_Demo-6366F1">
</p>

---

## ðŸ“Œ Overview

Bookkeeping and CPA firms lose **10â€“20 hours every week** to repetitive manual work â€” keying
invoices, chasing receipts, writing client updates and eyeballing transactions for errors.

**PixlForge AutoBooks AI** is a fleet of **5 connected automations** that run around the clock.
[Anthropic **Claude**](https://www.anthropic.com) handles the judgement-heavy steps (extraction,
classification, anomaly reasoning, report writing) while self-hosted **n8n** orchestrates the
integrations firms already use â€” QuickBooks, Xero, Google Sheets, Gmail and Slack.

> ðŸ’¡ **The business case:** `15 hrs/week Ã— $50/hr Ã— 4.33 weeks â‰ˆ $3,250 saved every month` â€” the
> engagement typically pays for itself in the first month, then runs autonomously.

<p align="center">
  <img src="assets/thumbnail_main.png" alt="AI Bookkeeping Agent" width="80%">
</p>

---

## âœ¨ What it can do (benefits)

| | Benefit |
|---|---|
| ðŸ§¾ | **Zero-touch invoice entry** â€” emailed invoices are read, categorized and filed automatically, with duplicates blocked before theyâ€™re paid. |
| ðŸ“ˆ | **Effortless client reporting** â€” branded weekly financial reports written by AI and emailed every Monday. |
| ðŸš¨ | **Always-on fraud & error detection** â€” nightly anomaly scans catch spikes, new vendors and double-payments. |
| ðŸ¤ | **Instant client onboarding** â€” a web form spins up a profile, welcome email, Slack channel and check-in. |
| ðŸ§® | **No more tax-season scramble** â€” per-client readiness scores flag missing items early. |
| ðŸ”’ | **Your data stays yours** â€” self-hosted by default; nothing has to leave the clientâ€™s infrastructure. |

---

## ðŸ“¸ Real screenshots

> These are **live captures** from the running Streamlit dashboard and the actual n8n editor â€” not mockups.

<table>
  <tr>
    <td width="50%"><img src="assets/screenshot_01_dashboard.png"><br><sub><b>Command Center</b> â€” KPIs, revenue & expense analytics, live AI activity log</sub></td>
    <td width="50%"><img src="assets/screenshot_02_invoice_flow.png"><br><sub><b>n8n workflow</b> â€” the Smart Invoice Processor, fully connected</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="assets/screenshot_03_ai_report.png"><br><sub><b>Weekly AI Report</b> â€” branded, Claude-written client report</sub></td>
    <td width="50%"><img src="assets/screenshot_04_anomaly.png"><br><sub><b>Anomaly Detection</b> â€” severity-scored feed with AI explanations</sub></td>
  </tr>
  <tr>
    <td width="50%"><img src="assets/screenshot_05_chat.png"><br><sub><b>Ask the AI Agent</b> â€” natural-language Q&A over the ledgers</sub></td>
    <td width="50%"><img src="assets/screenshot_06_invoices.png"><br><sub><b>Invoice Intelligence</b> â€” AI-tagged, duplicate-checked, color-coded</sub></td>
  </tr>
</table>

---

## âš™ï¸ The 5 automations

| # | Workflow | What it does |
|---|----------|--------------|
| 1 | **Smart Invoice Processor** | Email/webhook â†’ Claude extracts vendor, amount, date & tax â†’ duplicate check â†’ logs to Sheets + Airtable â†’ categorizes â†’ notifies the accountant. |
| 2 | **Weekly AI Client Report** | Every Monday 8 AM â†’ loops clients â†’ computes revenue/expense/net â†’ Claude writes a branded summary + 3 insights + 2 recommendations â†’ emails it â†’ logs it. |
| 3 | **AI Anomaly Detection** | Nightly â†’ compares last 24 h vs. 90-day baseline â†’ Claude flags spikes / new vendors / duplicate payments with a severity score â†’ priority alert. |
| 4 | **New Client Onboarding** | Web form â†’ creates profile â†’ Claude writes a personalized welcome â†’ email + checklist + Slack channel + 7-day check-in. |
| 5 | **Tax Season Readiness** | Monthly â†’ checks missing receipts & uncategorized txns â†’ Claude scores readiness 0â€“100 â†’ flags high-risk clients before deadlines. |

Each workflow is a **valid, importable `n8n` JSON** with error-handling lanes and fully-configured Claude API nodes.

---

## ðŸš€ Innovative features (industry-first)

- **AI Client Health Scoreâ„¢** â€” a weekly 0â€“100 score per client blending payment timeliness, expense growth, cash-flow stability and anomaly history.
- **Duplicate Invoice Neural Detection** â€” semantic matching catches the *same* invoice re-billed with a slightly different amount or date.
- **Tax Season Readiness Radar** â€” per-client quarterly readiness % with the exact missing items flagged.
- **Smart Vendor Fingerprinting** â€” learns each clientâ€™s known vendors and auto-flags new/unknown ones for approval.
- **Natural-Language Financial Q&A** â€” â€œwhich clients spiked >20% this month?â€ answered in seconds. No SQL, no pivot tables.
- **Multi-Software Auto-Sync** â€” QuickBooks, Xero, Wave, FreshBooks + Google Sheets. Clients keep the tools they already use.

---

## ðŸ† Why this is best-in-class

- âœ… **Real, not tutorial-grade** â€” the n8n workflows import and run; the dashboard is a production-quality Streamlit app.
- âœ… **AI where it matters** â€” Claude does the reasoning; n8n does the plumbing. Clean separation, production patterns.
- âœ… **Runs with zero setup** â€” full **DEMO/mock mode** means anyone can try it without an API key or cost.
- âœ… **Privacy-first** â€” self-hosted; secrets in `.env`/credentials; Anthropic doesnâ€™t train on API data.
- âœ… **Complete deliverable** â€” workflows, dashboard, branded emails, sample data, PDF report and docs.

---

## ðŸ§° Tech stack

<p>
  <img src="https://img.shields.io/badge/n8n-EA4B71?logo=n8n&logoColor=white">
  <img src="https://img.shields.io/badge/Anthropic_Claude-D97757?logo=anthropic&logoColor=white">
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white">
  <img src="https://img.shields.io/badge/Plotly-3F4F75?logo=plotly&logoColor=white">
  <img src="https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white">
  <img src="https://img.shields.io/badge/Pillow-image_gen-4B8BBE">
  <img src="https://img.shields.io/badge/ReportLab-PDF-00897B">
  <img src="https://img.shields.io/badge/Faker-sample_data-2C3E50">
</p>

| Layer | Tool |
|---|---|
| Automation engine | n8n (self-hosted) |
| AI / reasoning | Anthropic Claude (`claude-sonnet-4`) |
| Dashboard | Streamlit + Plotly |
| Data store | Google Sheets (demo) / Airtable (prod) |
| Email / alerts | Gmail Â· SendGrid Â· Slack |
| Reports & assets | ReportLab (PDF) Â· Pillow (thumbnails) |

---

## ðŸ“‚ Project structure

```
bookkeeping-ai-agent-demo/
â”œâ”€â”€ n8n-workflows/      5 importable n8n workflow JSONs (+ builder)
â”œâ”€â”€ dashboard/          Streamlit app (5 tabs, theme, components)
â”œâ”€â”€ sample-data/        realistic US data generator + JSON
â”œâ”€â”€ email-templates/    3 branded HTML emails
â”œâ”€â”€ fiverr-assets/      thumbnails, banner, screenshots (+ generators)
â”œâ”€â”€ fiverr-report/      portfolio PDF (+ generator)
â”œâ”€â”€ assets/             README visuals
â”œâ”€â”€ README.md Â· SETUP.md Â· .env.example Â· LICENSE
```

## â–¶ï¸ Quick start

```bash
# 1) sample data
python sample-data/generate_data.py

# 2) dashboard (DEMO mode â€” no API key needed)
cd dashboard && pip install -r requirements.txt && streamlit run app.py

# 3) n8n â€” import any file from /n8n-workflows
npx n8n start
```

For live Claude responses, copy `.env.example` â†’ `.env` and set `ANTHROPIC_API_KEY`.
Full client-deployment guide in **[SETUP.md](SETUP.md)**.

> ðŸ”’ **Note:** This public repository is a **showcase**. The complete, production source is
> maintained privately and delivered as part of an engagement.

---

## ðŸ‘‹ About PixlForge

PixlForge designs production-grade AI automation for finance, accounting and operations teams.

- ðŸ“§ **Email:** [info@pixlforgestudio.in](mailto:info@pixlforgestudio.in)
- 📬 **Direct:** [namancric18@gmail.com](mailto:namancric18@gmail.com)
- ðŸŒ **Portfolio:** [pixlforgestudio.in](https://pixlforgestudio.in/)
- ðŸ’¼ **LinkedIn:** [Naman Jain](https://www.linkedin.com/in/naman-jain-a41893266)

> ðŸ’¬ Want this for your firm? **Message me for a free workflow audit** â€” Iâ€™ll map your current
> process and recommend exactly which automations to start with.

---

## ðŸ“œ License

See **[LICENSE](LICENSE)**. This is a portfolio / demo project â€” free to view and evaluate, not for
redistribution or resale. Commercial deployment is available as a service engagement.

---

<p align="center">
  <sub>âš¡ Built with full focus and production discipline Â· <b>Developed by Naman Jain</b> Â· Â© PixlForge</sub>
</p>
