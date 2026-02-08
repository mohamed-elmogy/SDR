# 📧 AI Multi-Agent Sales Email Automation

This project demonstrates a **multi-agent AI workflow** that
automatically:

-   Generates multiple cold sales email drafts\
-   Selects the best performing draft\
-   Generates a high-converting subject line\
-   Converts the email into HTML format\
-   Sends the email via SendGrid

Built using **OpenAI Agents SDK**, **SendGrid**, and **Python Async
execution**.

------------------------------------------------------------------------

## 🚀 Features

✅ Multi-agent architecture\
✅ Professional / Humorous / Concise email generation\
✅ Automated draft evaluation and selection\
✅ Subject line optimization\
✅ HTML email formatting\
✅ Automatic email sending via SendGrid\
✅ Tool-based agent orchestration\
✅ Async execution with tracing

------------------------------------------------------------------------

## 🧠 Architecture Overview

    Sales Manager Agent
            ↓
     ┌───────────────┐
     │ Sales Agents  │
     │---------------│
     │ Professional  │
     │ Engaging      │
     │ Busy          │
     └───────────────┘
            ↓
    Select Best Draft
            ↓
    Email Manager Agent
            ↓
    Subject Writer → HTML Converter → Send Email

------------------------------------------------------------------------

## 📦 Tech Stack

-   Python 3.9+
-   OpenAI Agents SDK
-   GPT Models (gpt-5.2, gpt-4o-mini)
-   SendGrid Email API
-   Asyncio
-   python-dotenv

------------------------------------------------------------------------

## 📂 Project Structure

    project/
    │
    ├ main.py
    ├ .env
    ├ requirements.txt
    └ README.md

------------------------------------------------------------------------

## ⚙️ Installation

### 1️⃣ Clone Repository

    git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
    cd YOUR_REPO

------------------------------------------------------------------------

### 2️⃣ Create Virtual Environment

    python -m venv venv

Activate:

**Windows**

    venv\Scripts\activate

**Linux / Mac**

    source venv/bin/activate

------------------------------------------------------------------------

### 3️⃣ Install Dependencies

    pip install -r requirements.txt

------------------------------------------------------------------------

## 🔑 Environment Variables

Create a `.env` file in root folder:

    OPENAI_API_KEY=your_openai_key
    SENDGRID_API_KEY=your_sendgrid_key

------------------------------------------------------------------------

## 📧 SendGrid Setup

1.  Create SendGrid account\
2.  Generate API Key\
3.  Verify sender email\
4.  Replace inside code:

``` python
from_email = Email("YOUR_VERIFIED_EMAIL")
to_email = To("RECIPIENT_EMAIL")
```

------------------------------------------------------------------------

## ▶️ Running The Project

    python main.py

------------------------------------------------------------------------

## 📝 Example Input

``` python
message = "Send out a cold sales email addressed to Dear CEO from Alice"
```

------------------------------------------------------------------------

## 🛠 Agents Description

### 🧑‍💼 Sales Agents

  Agent          Style
  -------------- --------------------
  Professional   Corporate, serious
  Engaging       Humorous, witty
  Busy           Short and direct

------------------------------------------------------------------------

### 📬 Email Manager Agent

Responsible for:

-   Writing subject line\
-   Converting email to HTML\
-   Sending email via SendGrid

------------------------------------------------------------------------

## 🔍 Workflow Logic

### Step 1 --- Draft Generation

Sales Manager calls all 3 sales agents

### Step 2 --- Evaluation

Best draft is selected automatically

### Step 3 --- Handoff

Draft passed to Email Manager

### Step 4 --- Email Processing

Subject → HTML → Send Email

------------------------------------------------------------------------

## 📊 Observability

Uses tracing:

``` python
with trace("Automated SDR"):
```

------------------------------------------------------------------------

## 🧪 Customization

### Change Email Tone

Edit agent instructions:

``` python
instructions1 = "..."
```

------------------------------------------------------------------------

### Add More Sales Agents

Create new agent + register as tool.

------------------------------------------------------------------------

### Change Models

Example:

``` python
model="gpt-5.2"
```

------------------------------------------------------------------------

## ⚠️ Security Notes

❌ Never commit `.env`\
❌ Never expose API keys\
✅ Use GitHub Secrets for production

------------------------------------------------------------------------

## 📌 Requirements Example

Create `requirements.txt`:

    openai
    sendgrid
    python-dotenv
    asyncio

------------------------------------------------------------------------

## 🤝 Contributing

Pull requests are welcome.

------------------------------------------------------------------------

## 📜 License

MIT License

------------------------------------------------------------------------

## 👤 Author

Ahmed Elmogy\
AI Engineer / Developer
