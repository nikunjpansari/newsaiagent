# News AI Agent

A **CrewAI-based News AI Agent** that leverages **Google Gemini Pro** for advanced language understanding and **SerperAPI** for real-time search results. This project fetches breaking news articles, summarizes them, and answers user queries about current events.

---

## 🚀 Features

- **Real-time news search** via SerperAPI (Google Search)
- **Contextual understanding & summarization** using Google Gemini Pro
- **Customizable agent workflows** powered by CrewAI
- easy-to-extend architecture for adding new data sources or LLM integrations
- Authentication & rate-limit handling for all APIs

---

## 🏗️ Architecture


1. **User UI** (CLI / Web) sends a query to the CrewAI Agent.  
2. **CrewAI Agent** orchestrates:
   - Calls **SerperAPI** for up-to-date search results.
   - Feeds raw content to **Google Gemini Pro** for summarization, Q&A, or classification.
3. **CrewAI Agent** returns processed answers or summaries back to the user.

---

## 📥 Getting Started

### Prerequisites

- Python 3.10+  
- `pip` for dependency management  
- Valid API keys for:
  - [Google Gemini Pro](https://cloud.google.com/vertex-ai/docs/generative-ai/gemini-overview)  
  - [SerperAPI](https://serper.dev/)  

### Installation

1. **Clone the repo**  
   ```bash
   git clone https://github.com/your-username/news-ai-agent.git
   cd news-ai-agent

2. **Create & activate a virtual environment**  
   ```bash
    python3 -m venv .venv
    source .venv/bin/activate      # Linux / macOS
    .venv\Scripts\activate         # Windows

3. **Install dependencies**  
   ```bash
    python3 -m venv .venv

⚙️ Configuration
Create a .env file in the project root with the following variables:

# Google Gemini Pro (Vertex AI)
GOOGLE_API_KEY=your_gcp_api_key

# SerperAPI
SERPER_API_KEY=your_serper_api_key

⚡ Usage
1. Run as a CLI
   ```bash
   python crew.py
