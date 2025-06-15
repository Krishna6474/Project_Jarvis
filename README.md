# JARVIS AI Assistant

JARVIS is an advanced AI assistant that combines voice and text interfaces, task and reminder management, and intelligent conversation using state-of-the-art LLMs (Google Gemini, Groq Llama3) and vector search for context. It features a modern web UI and can also run in continuous voice mode.

## Features

- **Conversational AI**: Chat with JARVIS using natural language (text or voice).
- **Task Management**: Add, list, and update tasks with priorities and due dates.
- **Reminders**: Set and receive reminders.
- **Contextual Memory**: Vector search for previous conversations and context.
- **Web Interface**: Modern, interactive web UI with voice support.
- **Voice Mode**: Wake-word detection and continuous listening (desktop only).
- **Agentic Reasoning**: Uses LangChain agents for advanced task handling.

## Requirements

- Python 3.8+
- Node.js (optional, for frontend development)
- API keys for [Google Gemini](https://ai.google.dev/) and [Groq](https://console.groq.com/)

## Setup

1. **Clone the repository**

   ```bash
   git clone <your-repo-url>
   cd Jarvis_Project
   ```

2. **Install Python dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Set API Keys**

   Export your API keys as environment variables:

   ```bash
   export GEMINI_API_KEY='your_gemini_api_key'
   export GROQ_API_KEY='your_groq_api_key'
   ```

   Or set them in your shell profile (`.bashrc`, `.zshrc`, etc).

4. **Run the Backend**

   ```bash
   python app.py
   ```

   The Flask server will start at [http://localhost:4000](http://localhost:4000).

5. **Access the Web Interface**

   Open your browser and go to [http://localhost:4000](http://localhost:4000).

## Usage

- **Web UI**: Use the chat box to interact with JARVIS. You can type or use the microphone button for voice input.
- **Voice Mode**: (Desktop only) Run `jarvis_ai.py` directly for continuous wake-word listening.
- **APIs**: The backend exposes REST endpoints for conversation, tasks, reminders, and search.

## Project Structure

```
Jarvis_Project/
├── app.py                # Flask backend server
├── jarvis_ai.py          # Main Jarvis AI logic
├── requirements.txt      # Python dependencies
├── static/               # Frontend static files (HTML, CSS, JS)
├── jarvis_data/          # Data storage (created at runtime)
└── README.md
```

## Notes

- For best voice experience, use Chrome or Edge browsers.
- Data is stored in `jarvis_data/` as Excel and pickle files.
- Make sure your API keys are valid and have sufficient quota.

## License

MIT License

