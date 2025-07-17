# 🛠️ n8n + Slack Webhook Automation

This is a simple demo project showing how to use **n8n** to automate sending Slack messages from an incoming **Webhook** request.

---

## 🔷 📌 **Project Overview**

✅ **Goal:**  
Receive data (name, code) from a Webhook and automatically send it as a formatted message to a specific Slack channel.

✅ **Tools Used:**
- [n8n](https://n8n.io) (Low-code Automation Tool)
- Slack (Communication Platform)

---

## 🚀 **How It Works**

1. **Webhook Node**
   - Receives a POST request containing an array of objects with `name` and `code`.

2. **Slack Node**
   - Iterates through the array.
   - Sends each item as a formatted message to the selected Slack channel.
     
**Project screens**
-------------

<code> <img src="/screenshot/n8n.jpg" width="190" height="380" alt="auth screen"> </code>

-------------
---

## 💡 **Example Input JSON**

```json
[
  {
    "name": "First item",
    "code": 1
  },
  {
    "name": "Second item",
    "code": 2
  }
]

```
🔔 Example Slack Message Output
name: First item
code: 1
Automated with this n8n workflow

name: Second item
code: 2
Automated with this n8n workflow

Import Workflow

Open n8n.

Click Import and select the provided MySlackWebhookWorkflow.json.

Set up Slack Credential

In Slack Node ➔ Add your Slack App Credential to allow message posting.

Copy Webhook URL

From Webhook Node ➔ copy Test URL or Production URL.

Send Test Data

Use Postman or curl to send the example input JSON to your Webhook URL.

Check Slack

The messages should appear automatically in your selected Slack channel.

🎯 Use Cases
✅ Notify team on new user registration
✅ Send form submissions directly to Slack
✅ Real-time alerts for sales or payments

👤 Author
Name: Salim Derradj

Role: Flutter and Web Developer | Automation Enthusiast

LinkedIn: [https://www.linkedin.com/in/salim-derradj-5568a526a/]









