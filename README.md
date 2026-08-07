# AI Ticket Classifier & Auto Routing

## Overview

This workflow automatically classifies customer support tickets using OpenAI, then routes them through a Switch node and stores the structured results in Google Sheets.

---

## Features

- AI-powered ticket classification
- Automatic priority detection
- Department routing
- Google Sheets integration
- Built with n8n

---

## Technologies

- n8n
- OpenAI
- Google Sheets
- Webhook
- Switch Node

---

## Workflow
```mermaid
flowchart LR
    A[Webhook] --> B[AI Agent]
    B --> C[Switch]
    C --> D[Google Sheets]
```

---

### Workflow Screenshot

![Workflow](AI-Ticket-Classifier-Workflow.png)


---

## Output Example

| Category | Priority | Department |
|----------|----------|------------|
| Billing | High | Finance |

---

## Import

Follow these steps to use this workflow in n8n:

1. Download `AI Ticket Classifier & Auto Routing.json` from this repository.
2. Open your n8n instance.
3. Click **Import from File**.
4. Select the downloaded JSON file.
5. Configure your OpenAI API credentials.
6. Configure your Google Sheets credentials.
7. Execute the workflow and test it using a webhook request.


## Requirements

Before using this workflow, make sure you have:

- n8n v1.x
- OpenAI API Key
- Google Sheets credentials
- Google OAuth configured

- ## License

MIT License
