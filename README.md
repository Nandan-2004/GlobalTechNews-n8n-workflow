# 🌍 GlobalTechNews - n8n Workflow

This repository contains an **n8n workflow** that fetches the latest **technology news** every 90 minutes, summarizes it using **Google Gemini**, and sends the summary to a **Telegram channel**.

---

## ✅ Features
- Fetches top tech headlines from **NewsAPI**.
- Summarizes articles into **3 bullet points** using **Gemini LLM**.
- Sends formatted messages to **Telegram** with title, summary, and link.

---

## ⚙️ Workflow Overview
1. **Schedule Trigger** – Runs every 90 minutes.
2. **HTTP Request** – Fetches top technology headlines from NewsAPI.
3. **Split Out** – Splits the articles array into individual items.
4. **Google Gemini Chat Model** – Provides LLM for summarization.
5. **Basic LLM Chain** – Summarizes the article content.
6. **Telegram** – Sends the summarized news to a Telegram group.

---

## 🔑 Requirements
- **n8n** installed locally or hosted.
- **NewsAPI Key** – [Get API Key](https://newsapi.org/).
- **Google Gemini API Key** – For summarization.
- **Telegram Bot Token** – Create via [BotFather](https://core.telegram.org/bots#botfather).

---

## 📦 Installation & Usage
1. Clone this repo:
   ```bash
   git clone https://github.com/YOUR_USERNAME/GlobalTechNews-n8n-workflow.git
   cd GlobalTechNews-n8n-workflow
   ```
2. Import the `globaltechnews-workflow.json` into n8n:
   - Go to **n8n Dashboard → Import → JSON File**.
3. Update credentials:
   - Add your **NewsAPI Key**, **Gemini Key**, and **Telegram Bot Token** in n8n.
4. Activate the workflow.

---

## 🖼 Workflow Diagram
```
Schedule → HTTP Request → Split Out → LLM Summarizer → Telegram
```

---

## 📜 License
This project is open-source under the MIT License.
