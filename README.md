# 🦤 LangChain SQL Chatbot

A Streamlit web application that allows you to interact with your **SQLite** or **MySQL** database using natural language queries, powered by **LangChain** and **GROQ's LLaMA3-8B**.

## 🚀 Features

- 🔗 Choose between SQLite (local `student.db`) or your own MySQL database
- 🤖 Chat with your SQL database using natural language
- 🧠 Powered by [LangChain](https://www.langchain.com/) and [GROQ LLaMA3](https://groq.com/)
- 🗄️ Auto-formatted prompts for SQL agents
- 📃 Caching with `st.cache_resource` for efficient database reuse
- 💬 Persistent chat history
- 🔐 Environment-based API key management

## 🧰 Tech Stack

- **Streamlit** – Frontend UI
- **LangChain** – SQL Agent and Prompt Handling
- **GROQ API** – LLM inference (LLaMA3-8B)
- **SQLAlchemy** – Database connection (SQLite/MySQL)
- **SQLite / MySQL** – Supported database engines

## 🖼️ Preview

[demo](https://your-screenshot-url-here.com) <!-- Add a screenshot if available -->

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/langchain-sql-chat.git
cd langchain-sql-chat
```

### 2. Create and activate a virtual environment

```bash
python -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Add environment variables

Create a `.env` file in the root directory:

```env
GROQ_API_KEY=your_groq_api_key
```

You can get your API key from [Groq's Developer Portal](https://console.groq.com/)

---

## 🧪 Running the App

```bash
streamlit run app1.py
```

---

## 🛠 Usage

1. Choose the database you want to connect to from the sidebar.
2. Enter your MySQL credentials (if applicable).
3. Provide your GROQ API key.
4. Start chatting and querying the database!

---

## 📂 File Structure

```
├── app1.py               # Main Streamlit app
├── student.db           # SQLite sample DB (if provided)
├── .env                 # API keys (not committed)
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

---

## 📜 Sample Queries

```plaintext
- Show all students in the database.
- How many courses are offered?
- List students who scored more than 90 in Math.
```

---

## 🧽 Requirements

- Python 3.8+
- GROQ API Key
- (Optional) MySQL database credentials

---

## 🔗 Reference

This project was inspired by the course: [Complete Generative AI Course with LangChain and HuggingFace](https://www.udemy.com/course/complete-generative-ai-course-with-langchain-and-huggingface/)
