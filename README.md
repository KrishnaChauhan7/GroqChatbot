# 💬 Groq Chatbot using Streamlit + Langchain

This is a simple LLM-powered chatbot built using:

- 🧠 **[Groq API](https://console.groq.com/)**
- ⚙️ **[Langchain](https://www.langchain.com/)**
- 🌐 **[Streamlit](https://streamlit.io/)** for UI
- 🚀 Deployed on **Streamlit Cloud**

👉 **Live Demo:** [Click here to chat!](https://groqchatbot-hwvzuumg83gdzqd92drbwm.streamlit.app/)

---

## 📁 Project Structure

```
Chatbots/
│
├── main.py             # Streamlit app logic
├── requirements.txt    # Required Python packages
└── .streamlit/
```

---

## ⚙️ How to Run Locally

1. **Clone the Repo:**

```bash
git clone https://github.com/your-username/groqchatbot.git
cd groqchatbot
```

2. **Create a Virtual Environment:**

```bash
python -m venv .venv
# Activate it:
# On Windows:
.venv\Scripts\activate
# On macOS/Linux:
source .venv/bin/activate
```

3. **Install Dependencies:**

```bash
pip install -r requirements.txt
```

4. **Set your API key:**

Create a `.streamlit/secrets.toml` file and paste:

```toml
GROQ_API_KEY = "your_groq_api_key_here"
```

5. **Run the Chatbot:**

```bash
streamlit run main.py
```

---

## 🌍 Deployment on Streamlit Cloud

1. Go to [Streamlit Cloud](https://streamlit.io/cloud)
2. Create a new app from your GitHub repo
3. Under “Secrets”, add:

```toml
GROQ_API_KEY = "your_actual_groq_key"
```

4. Click **Deploy**, and done! 🎉

---

## 🧠 How it Works

- Uses `ChatGroq` from `langchain_groq` to interact with Groq's hosted models (e.g. `llama3-8b-8192`)
- Input is taken from the Streamlit UI
- Model generates the response and it's displayed on the same page

---

## ✨ Example Models You Can Use

- `llama3-8b-8192`
- `mixtral-8x7b-32768`
- `gemma-7b-it` ❌ (Deprecated)

---

## 🧑‍💻 Author

👋 Made by Krishna Chauhan 
Email: krishnachauhannsut@gmail.com
Feel free to reach out for collab or suggestions!

---

## 📜 License

MIT License
