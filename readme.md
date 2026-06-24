# 🎙️ Jarvis: Next-Gen AI Voice & Desktop Assistant

Jarvis is a real-time, zero-latency voice and system automation assistant powered by **Gemini 2.5 Live API** and **OpenRouter**. Designed for developers and power users, Jarvis can hear your voice, see your screen, write/run code, control your operating system, and organize your files—all through natural conversation.

It features a custom desktop overlay interface built with Python/PySide6, as well as a modern web dashboard built with Next.js.

---

## ✨ Features

### 🎙️ Real-Time Voice Interaction
- **Gemini Live Audio**: Low-latency, bidirectional audio streaming using `gemini-2.5-flash-native-audio-preview`.
- **Seamless Typing & Speech**: Fluidly switch between voice input and text commands depending on your preference.

### 🖥️ OS & Desktop Control
- **System Actions**: Change volume, adjust brightness, toggle dark mode, reload tabs, capture screenshots, and manage open windows.
- **App Launcher**: Open any desktop application or URL by name (e.g., Chrome, VSCode, Spotify).
- **Files & Workspace**: List, create, rename, delete, or clean up your desktop and file directories automatically.
- **Mouse & Keyboard Simulation**: Move the cursor, click specific coordinates, double-click, drag, or type on screen.

### 👁️ Screen & Webcam Vision
- **Display Capture**: Captures your display to analyze code, debug errors, read articles, or assist you with whatever you are doing on screen.
- **Webcam Vision**: Utilizes your webcam to see and describe your surroundings.

### 📁 Advanced File Processing
- **Smart Handler**: Drop files directly into the assistant's UI to analyze them.
- **Supported Formats**:
  - **PDFs**: Extract text, summarize, or convert documents.
  - **Images**: Describe content, perform OCR, compress, resize, or convert formats.
  - **CSVs & Excel**: Sort, filter, calculate statistics, and summarize data.
  - **Code Files**: Review, write, optimize, test, or run scripts.
  - **Audio/Video**: Transcribe, trim, convert formats, or extract audio tracks.
  - **Archives**: List contents and extract archives automatically.

### 🧠 Persistent Long-Term Memory
- Silently remembers personal facts, project goals, habits, and preferences in a structured database to make every conversation personalized and contextual.

### 🌐 Web Dashboard & Tools
- **Next.js Frontend**: A modern web interface for configuring features, tracking memory, and monitoring task queues.
- **Specialized Integrations**: Built-in actions for YouTube controls, Google Flights finder, WhatsApp messaging, and Steam/Epic game installers.

---

## 🚀 Quick Start

### 📋 Prerequisites
- **Python**: version `3.11` or `3.12`
- **Node.js**: version `18+` (for the web frontend)
- **APIs**: A Gemini API key and an OpenRouter API key

### 🔧 1. Backend Installation & Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/syedroshan1526/Ai-voice-assistant-.git
   cd Ai-voice-assistant-
   ```

2. Install python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Initialize Playwright browser automation:
   ```bash
   playwright install
   ```

4. Create a configuration file at `config/api_keys.json`:
   ```json
   {
       "gemini_api_key": "YOUR_GEMINI_API_KEY",
       "openrouter_api_key": "YOUR_OPENROUTER_API_KEY"
   }
   ```

5. Run the Python assistant:
   ```bash
   python main.py
   ```

---

### 🌐 2. Web Frontend Setup (Optional)
Jarvis comes with a Next.js web application located under the `frontend/` directory.

1. Navigate to the frontend folder:
   ```bash
   cd frontend
   ```

2. Install npm packages:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

---

## 🛠️ Project Structure

```
├── actions/             # System integration modules (browser, file, mouse control)
├── agent/               # Autonomous execution planners and task queues
├── config/              # Keys and configurations
├── core/                # System instructions and prompt templates
├── frontend/            # Next.js web application
├── memory/              # Personal context and long-term memory system
├── main.py              # Main execution script (Gemini Live WebSocket loop)
├── ui.py                # Desktop overlay application layout
└── requirements.txt     # Python package requirements
```

---

## ⚠️ License

Licensed under **[Creative Commons BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)** (Personal & Non-Commercial Use Only).
⭐ **Star this repository to follow the development journey!**
