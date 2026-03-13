# homelist-ai-chatbot
AI chatbot for real estate website with lead capture to Google Sheets
# 🏠 Homie — AI Real Estate Chatbot for WordPress

A free, fully functional AI chatbot widget for real estate websites built on WordPress. Captures leads automatically into Google Sheets and sends email notifications — no monthly fees, no third-party platforms.

---

## ✨ Features

- 🤖 Smart guided conversation flow (Buy / Rent / PG / List)
- 📋 Auto lead capture form — Name, Phone, City, Requirement
- 📊 Saves leads to Google Sheets automatically
- 📧 Instant email notification for every new lead
- 🇮🇳 Bilingual — English & Hindi support
- 💰 100% Free — no monthly subscription
- ⚡ Works on any WordPress website

---

## 🛠️ Tech Stack

- **Frontend:** HTML, CSS, JavaScript (vanilla)
- **Backend:** Google Apps Script (Web App)
- **Database:** Google Sheets
- **Notifications:** Gmail via Google Apps Script
- **Platform:** WordPress (via WPCode plugin)

---

## 📁 Files

| File | Description |
|------|-------------|
| `homelist-widget-GITHUB.html` | Chat widget — paste into WordPress footer |
| `homelist-apps-script-GITHUB.js` | Google Apps Script — handles Sheet & Email |
| `README.md` | This file |

---

## 🚀 Setup Guide

### Step 1 — Google Sheet
1. Go to [sheets.google.com](https://sheets.google.com)
2. Create a new sheet named `Homelist Leads`
3. Copy the sheet URL

### Step 2 — Google Apps Script
1. Go to [script.google.com](https://script.google.com)
2. Create a new project
3. Paste contents of `homelist-apps-script-GITHUB.js`
4. Replace placeholders:
   - `YOUR_EMAIL@gmail.com` → your email
   - `YOUR_GOOGLE_SHEET_URL` → your sheet URL
5. Click **Deploy → New Deployment → Web App**
6. Set: Execute as **Me** | Access: **Anyone**
7. Copy the Web App URL

### Step 3 — WordPress Widget
1. Open `homelist-widget-GITHUB.html`
2. Replace placeholders:
   - `YOUR_GEMINI_API_KEY` → your Gemini API key (free at [aistudio.google.com](https://aistudio.google.com))
   - `YOUR_GOOGLE_APPS_SCRIPT_URL` → URL from Step 2
3. Install **WPCode** plugin in WordPress
4. Go to **WPCode → Header & Footer → Footer**
5. Paste the widget code → Save

---

## 💬 Conversation Flow

```
User opens chat
      ↓
Homie greets → asks Buy / Rent / PG / List
      ↓
Asks City → Property Type → BHK → Budget
      ↓
Lead form appears → User fills Name + Phone
      ↓
✅ Saved to Google Sheets + Email sent
```

---

## 📄 License

MIT License — free to use and modify for any project.

---

## 🙏 Credits

Built by Krati Bhatia for [Homelist.co.in](https://homelist.co.in) — a real estate portal based in Indore, India.
