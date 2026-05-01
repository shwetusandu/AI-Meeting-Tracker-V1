# AI Meeting Tracker - Interview FAQs

## 1. What problem does this project solve?

This project solves the common business issue where meeting notes are unstructured, action items are forgotten, owners are unclear, and follow-ups are delayed. It automates the conversion of meeting notes into actionable outputs.

---

## 2. What is AI Meeting Tracker?

AI Meeting Tracker is an automation solution that converts raw meeting notes into AI summaries, Jira tasks, Slack alerts, Gmail summaries, and Google Sheets logs.

---

## 3. What tools did you use?

- Make.com
- OpenAI
- Jira
- Google Sheets
- Slack
- Gmail
- Webhooks

---

## 4. Explain the workflow architecture.

Webhook Trigger
→ OpenAI Analysis
→ Parse JSON
→ Google Sheets Logging
→ Jira Issue Creation
→ Slack Notification
→ Gmail Alert

---

## 5. Why did you use Make.com?

Make.com provides fast no-code automation, easy integrations, routers, filters, scheduling, and scalable workflows.

---

## 6. Why did you choose JSON output from OpenAI?

JSON output is structured and easier to parse into downstream systems like Jira, Sheets, Slack, and Gmail. Plain text is harder to automate reliably.

---

## 7. How does Jira integration help?

AI extracts action items from meetings and automatically creates Jira tasks, ensuring execution and accountability.

---

## 8. What data is stored in Google Sheets?

- Timestamp
- Meeting Name
- Team
- Raw Notes
- AI Summary
- Action Items
- Risks
- Status
- Jira Ticket Number

---

## 9. How did you handle errors?

- Fixed Jira authentication issues using API token
- Used default assignee/reporter settings
- Used structured JSON parsing
- Simplified mandatory field mappings

---

## 10. What business value does this provide?

- Saves manual admin time
- Faster task creation
- Better accountability
- Improved stakeholder visibility
- Faster escalation of blockers

---

## 11. What challenges did you face?

- Jira 401 authentication errors
- Invalid assignee/reporter fields
- Unstructured AI outputs
- Multi-tool integration debugging

---

## 12. How did you solve Jira assignee errors?

Instead of sending dynamic names, Jira default assignment settings were used.

---

## 13. How did you improve Slack communication?

Slack Block Kit messages were designed to send clean ticket updates with issue keys and links.

---

## 14. How would you scale this project?

Version 2 roadmap:
- MCP AI agents
- Duplicate Jira detection
- Smart owner assignment
- Weekly leadership dashboards
- Sentiment analytics

---

## 15. What role did prompts play?

Prompts controlled extraction quality, structured JSON responses, summarization, risk detection, and reporting quality.

---

## 16. How does this project relate to Agile?

It supports standups, retrospectives, sprint planning, blocker tracking, and action accountability.

---

## 17. What did you learn from this project?

- Real-world automation design
- API authentication troubleshooting
- Prompt engineering
- Business workflow thinking
- Integration architecture

---

## 18. Why is this project portfolio-worthy?

It combines AI + Automation + Jira + Slack + Reporting + Business value in one real use case.

---

## 19. What would you improve next?

- Voice transcript ingestion
- Calendar integration
- Auto meeting scheduling
- AI decision agents
- Dashboard analytics

---

## 20. Give a 30-second summary.

I built an AI Meeting Tracker using Make.com and OpenAI that converts meeting notes into structured summaries, Jira tasks, Slack alerts, Gmail updates, and logs. It solves the business problem of weak follow-up after meetings.
