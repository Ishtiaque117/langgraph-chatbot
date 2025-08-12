# LangGraph Chatbot

A conversational AI chatbot built with [LangGraph](https://github.com/langchain-ai/langgraph), [LangChain](https://github.com/langchain-ai/langchain), and [Streamlit](https://streamlit.io/) for a modern, ChatGPT-like experience. Conversations are stored in a SQLite database, and you can switch between threads in the sidebar.

## Features

- ChatGPT-style interface using Streamlit
- Multiple conversation threads (each with a unique title)
- Persistent conversation history using SQLite
- Easy switching between conversations

## Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/langgraph-chatbot.git
   cd langgraph-chatbot
   ```

2. **Create a virtual environment and activate it:**
   ```bash
   python -m venv venv
   venv\Scripts\activate  # On Windows
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set your OpenAI API key:**
   - Create a `.env` file and add:
     ```
     OPENAI_API_KEY=your-api-key-here
     ```

5. **Run the app:**
   ```bash
   streamlit run frontend.py
   ```

## File Structure

- `frontend.py` — Streamlit UI and chat logic
- `backend.py` — LangGraph state management and SQLite checkpointing
- `requirements.txt` — Python dependencies
- `.gitignore` — Files and folders to ignore in git
- `.env` — Your environment variables (not tracked by git)

## License

MIT License