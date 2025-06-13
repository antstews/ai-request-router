## 🌳 Decision Tree – AI Request Router (Micro-Project 1)

This decision tree represents how an AI system classifies internal employee requests using GPT-based logic and routes them to the appropriate team.

---

### Root Node:
📨 **Incoming Request Submitted**

→ **Does the message clearly reference a known category keyword?**

- ✅ Yes → Proceed to Keyword Match Branch  
- ❌ No → Use AI Classification Branch

---

### 📚 Keyword Match Branch

→ Does the message contain:

- “payroll”, “benefits”, “vacation”, “leave” → 🏢 **HR**
- “password”, “device”, “login”, “account”, “email” → 🖥️ **IT**
- “lights”, “office”, “building”, “keycard”, “maintenance” → 🛠️ **Facilities**
- “invoice”, “payment”, “reimbursement”, “card” → 💳 **Finance**
- Other → Pass to AI Classifier for fallback analysis

---

### 🤖 AI Classification Branch

Use GPT prompt to interpret message context:
> *"You are an internal request classifier..."*  
Result returns a JSON with:
- `"category"` → Used to determine routing  
- `"confidence"` → Triggers fallback or human review if "low"  
- `"explanation"` → Stored in request log for transparency

---

### 📍Routing Actions

Based on the category:

- 📧 **Send confirmation email** to requester  
- 🧾 **Log request** in SharePoint or Excel (Team, Request, Date, Routing Path)  
- 📤 **Forward to assigned team inbox** or notify via Teams/Slack

---

### 🔁 Optional Handling for Unclear Requests

If `confidence = "low"` OR no category match:

→ Escalate request to a general Ops queue  
→ Include full request + AI explanation for human triage

---
