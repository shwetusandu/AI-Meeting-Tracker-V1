# AI Meeting Tracker - Prompt Library

## 1. Core Meeting Analysis Prompt (JSON Output)

```text
You are an expert Agile Delivery Assistant.

Analyze the following meeting transcript.

Return ONLY valid JSON.

{
  "summary":"",
  "action_items":"",
  "risks":"",
  "owners":"",
  "next_steps":""
}

Rules:
- Keep summary concise.
- Action items should be execution-focused.
- Risks should mention blockers or delays.
- Owners should list responsible people if mentioned.
- If missing data, return empty string.
- No markdown. No explanation.

Transcript:
{{notes}}
```

---

## 2. Improved Structured Prompt

```text
Analyze this meeting transcript.

Extract:
1. concise summary
2. tasks
3. owners
4. deadlines
5. blockers
6. delivery risks
7. sprint health sentiment

Return valid JSON only.
```

---

## 3. Weekly Dashboard Insight Prompt

```text
Analyze these weekly meeting records.

Provide:
1. Top recurring blocker
2. Team health summary
3. Delivery risks trend
4. Recommended management actions

Return concise business summary.
```

---

## 4. Jira Ticket Title Prompt

```text
Convert the action item below into a short professional Jira task title (max 10 words).

Action Item:
{{action_items}}
```

---

## 5. Slack Notification Summary Prompt

```text
Rewrite this meeting output into a concise Slack update using bullet points.

Input:
{{summary}}
{{action_items}}
{{risks}}
```

---

## 6. Executive Gmail Summary Prompt

```text
Create a professional executive email summary from the following meeting insights.

Include:
- Meeting purpose
- Key decisions
- Risks
- Required leadership attention
- Next steps
```

---

## 7. Sentiment / Health Prompt

```text
Based on this meeting transcript, classify sprint health:

Healthy / Watchlist / Critical

Give one-line reason only.
```

---

## 8. Duplicate Jira Detection Prompt (V2)

```text
Compare the new action item with existing Jira tasks.

Return:
- Duplicate
- Similar
- New Task

Existing tasks:
{{jira_tasks}}

New task:
{{action_items}}
```

---

## 9. Owner Recommendation Prompt (V2)

```text
Based on these open workloads, recommend the best owner for the new task.

Users:
{{team_workload}}

Task:
{{action_items}}
```

---

## 10. README Generator Prompt

```text
Create a professional GitHub README for an AI automation project.

Include:
Overview
Problem Solved
Architecture
Tools Used
Workflow Steps
Business Value
Screenshots Section
Future Improvements
```
