# 🎬 AI Video Assistant (Video Agent)

An intelligent Streamlit application that transcribes, summarizes, and answers questions about any given video link. Stop watching hour-long videos just to find one piece of information—let the AI do the heavy lifting for you.

## ✨ Features
* **Link-to-Text Transcription:** Automatically downloads audio from video links and transcribes it locally using [OpenAI's Whisper](https://github.com/openai/whisper).
* **Smart Summarization:** Generates quick, highly accurate summaries of the entire video content.
* **Interactive Q&A:** Chat directly with the video! Ask specific questions and get answers based strictly on the video's transcript.
* **Local Vector Database:** Uses [ChromaDB](https://www.trychroma.com/) for lightning-fast semantic search and retrieval (RAG).
* **Clean Web UI:** Built with [Streamlit](https://streamlit.io/) for a smooth, intuitive user experience.

## 🏗️ Architecture & Tech Stack
* **Frontend:** Streamlit
* **Transcription:** OpenAI Whisper & FFmpeg (via Pydub)
* **Orchestration & RAG:** LangChain (`langchain-chroma`, `langchain-core`)
* **Vector Database:** ChromaDB
* **LLM Provider:** Mistral / Sarvam (via API)

## 🚀 Getting Started

### Prerequisites
1. **Python 3.10+** (Recommended)
2. **FFmpeg:** Required for audio processing. 
   * *Windows:* Open a fresh terminal and run `winget install ffmpeg`. Restart your terminal after installing.

### Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YourUsername/video-agent.git](https://github.com/YourUsername/video-agent.git)
   cd video-agent
