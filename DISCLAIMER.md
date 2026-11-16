# ⚠️ Disclaimer & Liability Limitation

**Use at your own risk.** The code, workflows, and scripts in this repository (`n8n-chilipiper-hubspot-instant-routing-fallback-handler`) are provided for educational and architectural demonstration purposes.

## No Liability

The author and dhRobin Systems accept no responsibility or liability for any direct, indirect, incidental, or consequential damages that result from using, misusing, or deploying these scripts. This includes, without limitation, lost or delayed leads, missed meetings, leads assigned to the wrong or an unavailable SDR, duplicate or missing tasks, overwritten or incorrect contact data, unwanted outreach, regulatory claims arising from contacting leads, unintended disclosure of lead information, service interruptions, and API quota exhaustion.

## No Warranty

All software, n8n JSON blueprints, JavaScript modules and prompts are provided "AS IS", without warranty of any kind, express or implied. This includes, but is not limited to, warranties of merchantability, fitness for a particular purpose, and non-infringement.

No warranty is given that every failed routing event from Chili Piper, Calendly or HubSpot is received, recognised or parsed correctly (payload formats vary by account configuration and may change); that signature verification is compatible with your providers' signing methods; that round-robin, territory, capacity, out-of-office or cooldown logic produces the assignment you intend; or that task, note, contact and Slack writes succeed or happen in time to meet any service level.

## Production Testing Required

Always test thoroughly in an isolated staging environment, such as a HubSpot developer test account or sandbox, with `SANDBOX_MODE=true`, `DRY_RUN=true`, `CREATE_FALLBACK_TASKS=false` and `SEND_SLACK_ALERTS=false` enabled, before you connect live HubSpot, Chili Piper, Calendly or Slack credentials. Validate signature verification with real signed test requests, confirm the parser against real failed-routing payloads from each source, run a failure drill with your SDR team, and keep monitoring SLA adherence after go-live.

Treat every automated assignment, task and contact update as an operational action that your team must monitor and be able to correct.

## Third-Party APIs & Compliance

You alone are responsible for complying with the terms of service, rate limits, data privacy regulations (GDPR/CCPA and equivalents), and security policies of HubSpot, Chili Piper, Calendly, Slack and any connected services. That includes:

- telling leads, through your scheduling forms and privacy notice, how their data is used for follow-up when a booking fails;
- honouring consent, communication preferences, do-not-call registers and regional calling or messaging rules before SDRs make contact;
- keeping lead contact details out of Slack and other channels that shouldn't receive them;
- securing, rotating and restricting access to the HubSpot private app token, the Slack webhook URL, and the Chili Piper, Calendly and HubSpot signing secrets;
- limiting access to n8n execution data, which contains lead information, and applying a retention period that matches your policies;
- reviewing every automatically created or updated record.

## No Affiliation

HubSpot, Chili Piper, Calendly, Slack and n8n are trademarks of their respective owners. This project is independent and is not affiliated with, endorsed by, or sponsored by any of them. All people, companies, SDRs, identifiers, URLs and events in the fixtures and pinned data are fictitious.

## Not Professional Advice

Nothing in this repository constitutes legal, privacy, security, or financial advice. Consult qualified professionals for your specific circumstances.

---

Released under the MIT License. Copyright (c) 2026 DH Robin (dhRobin Systems). See [LICENSE](LICENSE).

Full text: DISCLAIMER.md · Licensed under the MIT License. License: MIT © 2026 dhRobin Systems · Provided as-is, see the disclaimer.
