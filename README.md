# 🧠 AI Request Router — A No-Code Routing Assistant

This micro-project is part of a 14-day AI sprint exploring $0 automation solutions using Microsoft Copilot Studio, Power Platform, and GPT-based classification. **The AI Request Router** analyzes natural language queries submitted by internal users (e.g., “I can’t access my pay stub”) and routes them to the correct team: HR, IT, Facilities, Finance, or Escalation.

It uses a combination of keyword logic and a smart classifier prompt to turn messy text into structured decisions—automatically.

---

## 🚀 What It Does

- Accepts incoming form/email/text requests from users  
- Attempts category classification via keyword match  
- Falls back to GPT-based analysis if unclear  
- Responds with a confirmation email or message  
- Logs the request with category, confidence, and explanation  
- Routes the request to the right team inbox or system

---

## 🧩 Built With

- Power Automate (free-tier logic flows)  
- OpenAI or Azure OpenAI API (for natural language classification)  
- Markdown + Obsidian (for system modeling & documentation)  
- Optionally SharePoint or Excel for request logs

---

## 📁 Project Structure

README.md | project summary + architecture |
prompt.md | GPT classification prompt |
decision-tree.md | logic map for routing paths |
flow-diagram.mmd | mermaid-based system diagram |
data-model.md | structured log schema |
responses.md | auto-reply templates (per catagory) |
reflections.md | sprint notes and learnings |

---

## ✍️ Why I Built This

Internal operations are overloaded with requests—and most aren’t urgent, just misrouted. This workflow proves that even without infrastructure or engineering resources, *you can build intelligent routing systems using free tools and smart prompt design.* It’s also a warm-up for deeper sprint projects focused on cybersecurity and Copilot UX.

---

## 💡 Future Enhancements

- Add UI to simulate input form or inbox  
- Improve prompt with role or urgency detection  
- Integrate with Microsoft Teams or Slack for alerts  
- Add metrics to track routing accuracy over time

---

Built by [@caduceus-dev](https://github.com/antstews) during the #NoDollarSprint  
