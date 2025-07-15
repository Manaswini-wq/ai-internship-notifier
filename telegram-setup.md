# 📩 Telegram Bot Setup – AI Internship Notifier

This document explains how the Telegram integration works in this project.

---

## ✅ Bot Creation (Using BotFather)

1. Open Telegram and search for `@BotFather`
2. Send `/start` and then `/newbot`
3. Give it a name (e.g., InternshipNotifierBot)
4. Choose a unique username (e.g., `@intern_notify_bot`)
5. BotFather will give you a **Bot Token** — copy this.

---

## 🔧 n8n Telegram Setup

1. Go to n8n → Click “Credentials” → Create New → `Telegram API`
2. Paste the **Bot Token**
3. In your workflow:
   - Add a **Telegram node** (e.g., “Send Message”)
   - Connect it after your Airtable or webhook node
   - Choose:
     - **Chat ID**: use your group or personal chat ID
     - **Message**: use expressions like:
       ```
       New Application Received:
       Name: {{$json["name"]}}
       Skills: {{$json["skills"]}}
       Interests: {{$json["interests"]}}
       ```

---

## 🧪 Testing

- Invite your bot to a group or chat
- Run the full flow (form submission → Airtable → Telegram)
- Confirm real-time messages are delivered

---

## 🔒 Notes

- To get your chat ID, message your bot and use:
- https://api.telegram.org/bot<YourBotToken>/getUpdates
- 
---

🎉 You now have real-time alerts from your automation directly inside Telegram!

- 
