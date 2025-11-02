---

## 🧠 Local LLM Chat App (Phi-3 with Ollama + Gradio)

A simple and privacy-focused **local AI chat application** built using **Ollama** and **Gradio**, powered by the **Phi-3** language model — all running **locally** on your system.

---

### 🚀 Features

* 💬 Interactive Chat UI using **Gradio**
* ⚡ Powered by **Microsoft Phi-3** model (lightweight and fast)
* 🔒 100% offline — no API keys or internet required
* 🧩 Easy to switch between Ollama models
* 🧠 Great for quick experiments, learning, or local assistants

---

### 🧰 Requirements

* **Python 3.10+**
* **Conda** or **virtualenv**
* **Ollama** installed and running locally
  👉 [Download Ollama](https://ollama.ai/download)

---

### 🧱 Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/<your-username>/local-phi3-chat.git
   cd local-phi3-chat
   ```

2. **Create and Activate Environment**

   ```bash
   conda create -n code_llama python=3.11 -y
   conda activate code_llama
   ```

3. **Install Dependencies**

   ```bash
   pip install gradio requests
   ```

4. **Pull the Phi-3 Model**

   ```bash
   ollama pull phi3
   ```

5. **Run Ollama Service**

   ```bash
   ollama serve
   ```

6. **Start the App**

   ```bash
   python app.py
   ```

---

### 💻 Usage

Once the app starts, open your browser at:

👉 **[http://127.0.0.1:7860](http://127.0.0.1:7860)**

Type a question or prompt — the **Phi-3** model will respond locally.

---

### 🧩 Switching Models

To use a different model, edit your `app.py`:

```python
'model': 'phi3'
```

Change it to any other model you have installed, like:

* `mistral:latest`
* `codellama:latest`
* `gemma:2b`
* `llama2:7b`

> ⚠️ Some models (like Llama 13B) need 16GB+ RAM. For lighter systems, stick with `phi3` or `mistral`.

---

### 🧠 Project Structure

```
📦 local-phi3-chat/
 ┣ 📜 app.py          # Main Gradio application
 ┣ 📜 README.md       # Documentation
 ┗ 📜 requirements.txt
```

---

### 🧾 Example Interaction

```
Prompt: Explain machine learning in simple terms.
Response: Machine learning is a way for computers to learn from data and improve automatically without being explicitly programmed.
```

---

### 📜 License

This project is open-sourced under the **MIT License** — free for personal and commercial use.


