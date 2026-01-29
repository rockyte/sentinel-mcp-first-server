# 🚀 My First Microsoft Sentinel MCP Server (VS Code + Official Triage Endpoint)

> **Author:** Tarik Elkhatib  
> **Focus:** Microsoft Sentinel + MCP + AI Security Automation  
> **Use Case:** SOC Triage + Alert Trend Dashboards  
> **Status:** Working ✅

---

## 📌 Overview

The **Model Context Protocol (MCP)** is transforming how security teams interact with platforms like Microsoft Sentinel.

Instead of manually writing KQL and clicking through portals, MCP enables an AI agent (Copilot, Claude, etc.) to:

- Run Sentinel queries through tools  
- Summarize alert activity automatically  
- Generate dashboards and reports  
- Accelerate SOC triage workflows  

This repo documents my first successful Microsoft Sentinel MCP integration using the **official hosted Triage MCP server**.

---

## ✅ Sentinel MCP Endpoint Used

Since Sentinel Data Lake was not enabled in my tenant, I used the official hosted endpoint:

```
https://sentinel.microsoft.com/mcp/triage
```

---

## ⚙️ MCP Server Configuration (`mcp.json`)

```json
{
  "servers": {
    "my-mcp-server-b4dbbeec": {
      "url": "https://sentinel.microsoft.com/mcp/triage",
      "type": "http"
    }
  }
}
```

---

## 📊 Real Use Case: Weekly Alert Activity Dashboard

Prompt example:

> “Build me a web activity chart over the last week”

The agent executed Sentinel triage queries and generated an interactive dashboard with hover tooltips, legends, and severity insights.

---

## 📂 Repo Structure

```
sentinel-mcp-first-server/
│
├── README.md
├── mcp.json
└── screenshots/
    ├── mcp-running.png
    ├── agent-query.png
    ├── dashboard-final.png
```

---

## 🛡️ Lessons Learned

✅ Start with the triage endpoint if Data Lake is not enabled  
✅ Tenant authentication matters  
✅ MCP unlocks conversational SOC automation instantly  

---

## 🚀 Next Enhancements

- Insider Threat Agent Packs  
- Scheduled Sentinel MCP Weekly Reports  
- Sentinel + Defender + Purview Correlation  
- SOC Playbooks with AI-driven triage workflows  

---

⭐ If you found this useful, feel free to fork or adapt!

