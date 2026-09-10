# 🎙️ AI Voice Agent - Appointment Booking Assistant

An end-to-end conversational AI Voice Agent built using **ElevenLabs Conversational AI** and **n8n**, integrated with **Google Sheets** for real-time automated appointment booking.

## 🚀 Architecture & Flow
1. **User Voice Call** → ElevenLabs AI Voice Agent
2. **Tool Call** → Webhook trigger to n8n Workflow
3. **Data Storage** → Google Sheets (Appends booking details)
4. **Response** → Returns real-time confirmation back to the Voice Agent

## 📋 Features
- **Natural Voice Interaction:** Uses ElevenLabs Agent setup with custom System Prompts and Knowledge Base.
- **Smart Date Parsing:** Converts relative dates (e.g., "tomorrow") and standardizes times to 24-hour format (`Asia/Karachi` timezone).
- **Automated Workflow:** n8n Webhook receives parameters (`customer_name`, `phone_number`, `date`, `time`) and logs them seamlessly into Google Sheets.

## 🛠️ Tech Stack
- **Voice AI:** ElevenLabs Conversational AI
- **Automation Engine:** n8n (Cloud Workflow)
- **Database / Storage:** Google Sheets API

### n8n Webhook & Google Sheets Workflow
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2b1d20f3-56c2-41f6-ab86-8f97e9795baa" />

### ElevenLabs
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0006de94-b334-4a4f-bb21-7eb8540f4c90" />

### AI Voice Agent Setup
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dae85803-62d2-45b1-947a-c462c26d1e34" />



https://elevenlabs.io/app/talk-to?agent_id=agent_3401m20ssp3mecd8gfx7p5g4t70z&branch_id=agtbrch_0401m20ssq8qf7ks5n1fe9bse714


**AI-powered appointment assistant built with ElevenLabs Voice Agent, n8n automation, webhook integration, and Google Sheets for automated appointment booking and management.**


## 🔄 n8n Workflow

The `workflow.json` file contains the exported n8n workflow used to receive appointment details through a webhook and store them in Google Sheets.

### Workflow
Webhook → Google Sheets → Respond to Webhook
