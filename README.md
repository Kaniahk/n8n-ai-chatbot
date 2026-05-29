# 🚖 AI Taxi Booking Chatbot (n8n + LLM + WhatsApp)

## 📌 Project Overview
This project is an intelligent AI-powered taxi booking chatbot built using n8n (no-code automation platform).  
It simulates a real-world cab booking assistant that interacts with users via chat, processes booking requests, checks availability, and confirms orders automatically.

The chatbot is designed with structured conversation logic and integrates AI decision-making to handle different user intents like booking, FAQs, and order tracking.

---

## 🧠 Key Features

### 💬 Smart Conversation Handling
- Greets users and provides menu options
- Handles multiple intents:
  - 🚕 Booking Order
  - ❓ FAQs / Information
  - 📦 Check Order Status / Availability

### 🤖 AI Agent Logic
- Uses LLM (Groq / OpenAI) for natural language understanding
- Step-by-step data collection:
  - Customer Name
  - Taxi Type
  - Quantity / Booking details

### 📊 Data Integration
- Google Sheets used as database:
  - Store bookings
  - Check taxi availability
  - Retrieve order status

### 📦 Order Management
- Confirms booking if available
- Rejects booking if out of stock
- Stores only confirmed orders
- Tracks order status:
  - Confirmed
  - Rejected
  - Cancelled
  - Delivered

### 🔎 Additional Capabilities
- FAQ handling (booking time, payment, travel info)
- Real-time availability checking
- Friendly conversational tone (like real taxi apps)

---

## 🛠️ Tech Stack
- ⚙️ n8n (Workflow Automation)
- 🤖 LLM (Groq / OpenAI)
- 📊 Google Sheets API
- 💬 WhatsApp API (Messaging)
- 🧠 Simple Memory (Context Handling)

---

## 🔄 Workflow Logic

1. User sends message (e.g., "Book a cab")
2. Chat Trigger activates workflow
3. AI Agent identifies user intent
4. Based on intent:
   - Booking → Collect details → Check availability → Confirm order
   - FAQ → Provide quick answers
   - Order Check → Fetch data from Google Sheets
5. Response sent back to user via chat

---
## 📷 Workflow Screenshots

🔹 Main Workflow
<img width="1920" height="1080" alt="Screenshot (54)" src="https://github.com/user-attachments/assets/5623dd01-5cb3-4520-9836-6f6fafcdb6fa" />

🔹 AI Agent Setup
<img width="1920" height="1080" alt="Screenshot (56)" src="https://github.com/user-attachments/assets/bea5509b-cb67-4491-b9fc-2646dd1fcb91" />

🔹 Chat Output
<img width="1920" height="1080" alt="Screenshot (58)" src="https://github.com/user-attachments/assets/f3939dd2-057f-46cb-8567-b7991f8c144d" />

steps- <img width="1920" height="1080" alt="Screenshot (55)" src="https://github.com/user-attachments/assets/70a0153c-d0f8-440e-b355-0d10f37ee1ba" />
       <img width="1920" height="1080" alt="Screenshot (54)" src="https://github.com/user-attachments/assets/5623dd01-5cb3-4520-9836-6f6fafcdb6fa" />
       <img width="1920" height="1080" alt="Screenshot (57)" src="https://github.com/user-attachments/assets/07598aa0-1e57-4dec-a834-3a568be2df88" />

## 🚀 How to Run

1. Import the `workflow.json` file into n8n
2. Configure credentials:
   - Google Sheets API
   - WhatsApp API
   - LLM API (Groq / OpenAI)
3. Update Google Sheet structure
4. Activate workflow
5. Start chatting with the bot

---

## 🔐 Security Note
- API keys and credentials are not included
- Add your own credentials before running

---

## 🎯 Real-World Use Case
This project demonstrates:
- AI chatbot development without coding
- Workflow automation using n8n
- Real-world business use case (cab booking system)
- Integration of AI + database + messaging APIs

---

## 💡 Future Improvements
- Payment gateway integration
- Live GPS tracking
- Multi-language support
- Deployment with webhook UI




