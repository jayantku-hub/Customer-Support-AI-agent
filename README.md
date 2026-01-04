# AI Customer Support Agent (n8n + RAG)

This project demonstrates an AI-powered customer support workflow built using n8n, OpenAI, and Pinecone Vector Database.

The system automatically detects customer support emails, retrieves relevant company policies, and drafts accurate replies in Gmail with human approval.

## 🚀 Features
- Automatic customer support email detection
- Policy-based responses using Pinecone Vector DB (RAG)
- Gmail draft creation (no auto-send)
- Human-in-the-loop approval
- Scalable and safe AI workflow

## 🧠 Architecture
1. Gmail Trigger listens for new emails
2. AI classifies support vs non-support emails
3. Support emails are routed to AI Agent
4. Agent retrieves policies from Pinecone
5. Draft response is created in Gmail

## 🛠 Tech Stack
- n8n (Workflow Automation)
- OpenAI (LLM + Embeddings)
- Pinecone (Vector Database)
- Gmail API

## 📂 Workflows
- `customer-support-ai-agent.json` → Main automation
- `customer-support-vector-db.json` → Knowledge ingestion workflow

## ⚙️ Setup Instructions
1. Import workflows into n8n
2. Configure credentials:
   - Gmail
   - OpenAI
   - Pinecone
3. Upload customer policies using the vector DB workflow
4. Activate the main workflow

## 🔐 Safety
- Emails are never sent automatically
- All replies are drafted for human review
- Only company-approved knowledge is used

## 📌 Use Cases
- SaaS customer support
- Internal IT helpdesk
- Operations & support teams
- Startups scaling support

---

Built as a practical example of agentic AI in real business operations.
