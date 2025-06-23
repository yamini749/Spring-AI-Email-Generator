# 🌟 Spring AI Email Assistant

**Frontend:** React | **AI Engine:** Google Gemini API | **Backend:** Spring Boot | **Extension:** Chrome

---

## 🚀 Project Overview

An intelligent email management system powered by Spring Boot and Gemini AI. This assistant helps you handle emails more efficiently via:

-  A **Web Application** (React + Spring Boot)
-  A **Chrome Browser Extension**
-  **Google Gemini API Integration** for smart replies, summaries, and tone detection

---

## 🧠 Key Features

-  **AI-Generated Email Responses** — Instantly draft professional, context-aware replies
-  **Email Categorization** — Auto-classify emails (e.g., Work, Spam, Social)
-  **Summarization** — Convert lengthy email threads into brief, readable summaries
-  **Sentiment Detection** — Understand the tone of incoming messages

---

##  Tech Stack

| Layer         | Tech Stack                     |
|---------------|--------------------------------|
| Backend       | Spring Boot 3.2+, Java 17      |
| Frontend      | React                          |
| AI Engine     | Google Gemini API              |
| Email Client  | JavaMail API                   |
| Database      | H2 (Dev), PostgreSQL (Prod)    |
| Tools Used    | Maven, Postman                 |
| Extension     | Custom Chrome Extension (V3)   |

---

##  How to Run Locally

###  1. Clone the repository
```bash
git clone https://github.com/yamini749/Spring-AI-Email-Generator.git
cd Spring-AI-Email-Generator
```

###  2. Backend Setup (Spring Boot)
Create `application.yml` inside `src/main/resources/`

```yaml
server:
  port: 9191

gemini:
  api:
    url: YOUR_GEMINI_URL
    key: YOUR_GEMINI_API_KEY
```

Then build and run:
```bash
mvn clean install
mvn spring-boot:run
```

###  3. Frontend Setup (React)
If the frontend is in a separate folder:
```bash
cd frontend
npm install
npm start
```

---

##  Testing with Postman

Use the following endpoints to interact with the API:

| Endpoint                          | Method | Function                         |
|----------------------------------|--------|----------------------------------|
| `/api/email/generate`            | POST   | Generate AI-powered reply        |
| `/api/email/categorize`          | POST   | Categorize incoming email        |
| `/api/email/summarize`           | POST   | Summarize email content          |
| `/api/email/analyze-sentiment`   | POST   | Detect emotional tone            |
| `/api/email/schedule-followup`   | POST   | Schedule follow-up reminders     |

---

## 🌐 Chrome Extension

The Chrome Extension allows users to:
- Select email content
- Click to generate AI reply using backend API
- Paste and send with one click

📌 Built with Manifest V3 and integrated with the backend.

---

## 🤝 Contributions

Feel free to fork and contribute!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Commit changes (`git commit -m "Add feature"`)
4. Push (`git push origin feature/my-feature`)
5. Open a Pull Request

---

