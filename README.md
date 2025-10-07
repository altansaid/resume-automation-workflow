# 🧠 Resume Tailoring Automation (n8n Workflow)

This project automates the **resume tailoring process** using n8n.  
It enables job-specific, metric-driven, ATS-compatible **LaTeX resumes** powered by AI.

---

## 🚀 Features

- **Fully automated flow:** Triggered via Slack, end-to-end automation.
- **LaTeX resume generation:** AI-assisted content creation with PDF output.
- **n8n + OpenAI integration:** Uses prompt engineering and structured JSON master data.
- **GitHub Actions integration:** Automatically uploads and compiles resumes in GitHub.
- **Slack notification:** Sends generated PDF files to a Slack channel.
- **Version control:** Every resume version is tracked as a separate commit.

---

## 🧩 Architecture

Below is a simplified workflow diagram of the process:

```
Slack Trigger → Job Description → OpenAI Prompt → Resume Generator (LaTeX)
   ↓
GitHub Upload → GitHub Actions Build → PDF Output → Slack Notification
```

![Workflow Diagram](./assets/workflow-diagram.png)

---

## 🏗️ Technologies Used

| Technology         | Description                                                |
| ------------------ | ---------------------------------------------------------- |
| **n8n**            | Automation platform used to orchestrate the workflow.      |
| **OpenAI API**     | Generates resume bullet points and descriptions using GPT. |
| **Slack API**      | Handles triggers and notification delivery.                |
| **GitHub API**     | Manages automatic commits and file uploads.                |
| **LaTeX**          | Produces clean, professional, ATS-compliant resume PDFs.   |
| **GitHub Actions** | Compiles LaTeX files and generates PDFs automatically.     |

---

## ⚙️ Workflow Steps

### 1. Slack Trigger

A Slack command starts the workflow automatically.

### 2. Job Description Parsing

Extracts the job posting text and formats it for the AI prompt.

### 3. OpenAI Processing

GPT model generates resume bullet points following the X–Y–Z formula.

### 4. LaTeX Resume Creation

Outputs a complete LaTeX resume file preserving structure and style.

### 5. GitHub Upload

Automatically commits and pushes `.tex` file to a repository branch.

### 6. PDF Build & Slack Delivery

GitHub Actions compiles LaTeX → PDF and sends it back to Slack.

---

## 👨‍💻 Author

**Muhammed Said Altan**  
Software Developer
🌐 [saidaltan.com](https://saidaltan.com)  
📧 altansaid13@gmail.com  
💼 [LinkedIn](https://www.linkedin.com/in/saidaltan)

---

---

> 💡 Tip: If you plan to share the workflow publicly, remove all sensitive credentials before committing.
