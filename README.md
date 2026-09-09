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

**AI-powered appointment assistant built with ElevenLabs Voice Agent, n8n automation, webhook integration, and Google Sheets for automated appointment booking and management.**
