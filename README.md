# 🚖 AI Taxi Booking Chatbot (n8n + LLM + WhatsApp)

## 📌 Project Overview

An AI-powered taxi booking chatbot built using **n8n (workflow automation)** and **LLM integration (Groq/OpenAI)**.
The system simulates a real-world cab booking assistant that interacts with users via **WhatsApp**, processes booking requests, checks availability, and confirms orders automatically.

This project demonstrates how **no-code tools + AI** can be combined to build real-world automation systems.

---

## 🧠 Key Features

### 💬 Smart Conversation Handling

* Interactive chatbot with greeting and menu options
* Handles multiple user intents:

  * 🚕 Book a Taxi
  * ❓ FAQs / General Queries
  * 📦 Check Booking Status

### 🤖 AI-Powered Decision Making

* Uses LLM for natural language understanding
* Dynamically identifies user intent
* Collects booking details step-by-step:

  * Customer Name
  * Taxi Type
  * Booking Quantity / Details

### 📊 Data Integration (Google Sheets)

* Acts as a lightweight database:

  * Store confirmed bookings
  * Check taxi availability
  * Retrieve order status

### 📦 Order Management System

* Real-time availability check
* Booking outcomes:

  * ✅ Confirmed
  * ❌ Rejected (if unavailable)
* Order tracking system:

  * Confirmed / Cancelled / Delivered

### 🔎 Additional Capabilities

* FAQ automation (pricing, timing, services)
* Context-aware responses using memory
* Human-like conversational flow

---

## 🛠️ Tech Stack

* ⚙️ **n8n** – Workflow Automation
* 🤖 **LLM (Groq / OpenAI)** – NLP & Intent Detection
* 📊 **Google Sheets API** – Database
* 💬 **WhatsApp API** – User Interaction
* 🧠 **Memory Nodes** – Context Handling

---

## 🔄 Workflow Architecture

1. User sends message (e.g., *"Book a cab"*)
2. Chat trigger activates n8n workflow
3. AI agent detects intent
4. Workflow branches:

   * **Booking Flow** → Collect details → Check availability → Confirm
   * **FAQ Flow** → Instant response
   * **Order Status** → Fetch from database
5. Response sent back via WhatsApp

---

## 📷 Screenshots

### 🔹 Main Workflow

![Main Workflow](https://github.com/user-attachments/assets/5623dd01-5cb3-4520-9836-6f6fafcdb6fa)

### 🔹 AI Agent Setup

![AI Setup](https://github.com/user-attachments/assets/33dce5d2-f3fb-45fa-b1c3-7c37044456ba)

### 🔹 Chat Output

![Chat Output](https://github.com/user-attachments/assets/f3939dd2-057f-46cb-8567-b7991f8c144d)

---

## 🚀 How to Run

1. Import `workflow.json` into n8n
2. Configure API credentials:

   * Google Sheets API
   * WhatsApp API
   * Groq / OpenAI API
3. Update Google Sheet structure
4. Activate workflow
5. Start chatting with the bot

---

## 🔐 Security

* API keys are not included
* Use environment variables or n8n credentials

---

## 🎯 Use Case

This project showcases:

* AI chatbot development using **no-code tools**
* Real-world automation system (cab booking)
* Integration of **AI + APIs + database**
* Practical understanding of workflow orchestration

---

## 💡 Future Enhancements

* 💳 Payment gateway integration
* 📍 Live GPS tracking
* 🌐 Multi-language support
* ☁️ Deployment with webhook UI
* 📱 Mobile-friendly dashboard

---


---
