# 🔎 GitHub Profile Finder

A simple web-based GitHub Profile Finder that uses **Make, Webhooks, and the GitHub REST API** to retrieve public GitHub profile information and send a formatted profile report directly to the user's email.

## 🚀 Live Demo

<img width="1727" height="728" alt="Screenshot 2026-10-04 132058" src="https://github.com/user-attachments/assets/1c655d55-9253-4125-9bc6-0599d15a8722" />
<img width="976" height="902" alt="Screenshot 2026-10-07 001318" src="https://github.com/user-attachments/assets/5cc20a32-6c6f-4ff5-beeb-b3c1fc10fd0e" />
<img width="897" height="792" alt="Screenshot 2026-10-07 001259" src="https://github.com/user-attachments/assets/8f09a6e9-9e21-4deb-91e7-5f7a3beae862" />


---

## 📌 Overview

GitHub Profile Finder allows users to enter:

- GitHub Username
- Email Address

The application sends this information to a Make webhook. Make then uses the GitHub REST API to retrieve the requested public profile information and sends the results to the provided email address.

The project was built as a practical exercise in **workflow automation, REST APIs, webhooks, JSON data handling, and API integration**.

---

## ⚙️ How It Works

```text
User
  │
  │ GitHub Username + Email
  ▼
Web Interface
  │
  │ HTTP POST
  ▼
Make Webhook
  │
  │ Username
  ▼
GitHub REST API
  │
  │ Profile JSON
  ▼
Make
  │
  │ Format & Map Data
  ▼
Gmail
  │
  │ Profile Report
  ▼
User's Email
