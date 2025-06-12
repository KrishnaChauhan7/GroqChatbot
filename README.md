# 🧠 GROQ Chatbot using LangChain + Streamlit

This is a lightweight chatbot built using **LangChain**, **Groq LLMs**, and **Streamlit**. It can answer questions and engage in conversations — all through blazing fast inference powered by Groq!

---

## 🚀 Features

- ✅ Uses **Groq API** (LLMs like Mixtral, LLaMA3)
- ✅ Built with **LangChain** for managing the chain
- ✅ Easy interface with **Streamlit**
- ✅ Fully customizable and extensible
- ✅ Ready for deployment on **Streamlit Cloud**

---

## 🧰 Tech Stack

| Tool       | Role                         |
|------------|------------------------------|
| Python     | Core programming language    |
| LangChain  | LLM chaining and prompts     |
| Groq       | Fast inference (LLM backend) |
| Streamlit  | Web-based frontend           |

---

## 📁 Project Structure

```
Chatbots/
├── main.py               # Streamlit app
├── requirements.txt      # Project dependencies
└── .streamlit/
    └── secrets.toml      # API key config (optional)
```

---

## 🔑 Setup Instructions

### 1. Clone the repo

```bash
git clone https://github.com/your-username/groq-chatbot.git
cd groq-chatbot
```

### 2. Create Virtual Environment

```bash
python -m venv .venv
source .venv/bin/activate  # or `.venv\Scripts\activate` on Windows
```

### 3. Install Requirements

```bash
pip install -r requirements.txt
```

### 4. Add Your Groq API Key

You can do this in one of two ways:

#### Option A – Use Environment Variable

In `main.py`, make sure you access:

```python
import os
GROQ_API_KEY = os.getenv("GROQ_API_KEY")
```

Then set your API key:
```bash
export GROQ_API_KEY=your_key_here  # macOS/Linux
set GROQ_API_KEY=your_key_here     # Windows
```

#### Option B – Use `.streamlit/secrets.toml`

```toml
# .streamlit/secrets.toml
GROQ_API_KEY = "your_groq_api_key"
```

---

## ▶️ Run the App

```bash
streamlit run main.py
```

The app will open in your browser at:  
`http://localhost:8501`

---

## 🌐 Deploy to Streamlit Cloud (Free Hosting)

1. Push your project to a public GitHub repo
2. Visit [https://streamlit.io/cloud](https://streamlit.io/cloud)
3. Click "New App" and connect your GitHub
4. Choose the repo, set file path to `main.py`, and deploy!

---

## 📌 Example Prompt

> **Input:** "What is LangChain?"  
> **Output:** "LangChain is a framework for developing applications powered by language models..."

---

## 🤖 Models You Can Use

You can replace the model name depending on what Groq supports:

```python
model = ChatGroq(groq_api_key=GROQ_API_KEY, model_name="mixtral-8x7b-32768")
```

Visit: https://console.groq.com/docs/models

---

## 📄 License

MIT License — Free for personal and commercial use.

---

## 🙋‍♂️ Author

**Krishna Chauhan**  
👨‍💻 [GitHub](https://github.com/KrishnaChauhan7)  
📫 krishna.chauhan.ug22@nsut.ac.in
