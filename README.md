# 🌍 AI Travel Agency

> Powered by **LLAMA 4** + **Brave Search** + **Gradio UI**

An intelligent travel planning assistant powered by [PraisonAI Agents](https://pypi.org/project/praisonaiagents/), [LLAMA 4](https://groq.com), and Brave Search. This app leverages a team of autonomous AI agents to generate personalized travel plans, wrapped in an interactive Gradio UI.

---

## ✨ Features

- 🔎 Research destinations, local customs, and travel requirements
- ✈️ Find and compare flights
- 🏨 Recommend hotels and accommodations
- 📘 Design day-by-day itineraries
- 💡 Easy-to-use Gradio interface

---

## 🚀 Demo Preview

*(Add a screenshot or gif of the Gradio app here)*

---

## 🛠️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com//ai-travel-agency.git
cd ai-travel-agency
```

### 2. Create a Virtual Environment
```bash
python3.10 -m venv venv
source venv/bin/activate  # macOS/Linux
# OR
venv\Scripts\activate   # Windows
```

### 3. Install Dependencies
```bash
pip install -U "praisonaiagents[llm,mcp]" gradio python-dotenv
```

### 4. Set Up Environment Variables
Create a `.env` file in the root directory:
```ini
GROQ_API_KEY=your_groq_api_key
BRAVE_API_KEY=your_brave_api_key
```

---

## 🧠 How It Works

The app defines four specialized agents using the `praisonaiagents` framework:

- **Research Agent** – Information on attractions and local culture
- **Flight Agent** – Search and compare flights
- **Hotel Agent** – Suggest hotels based on budget
- **Itinerary Agent** – Build a day-by-day itinerary

These agents are executed in parallel using the `Agents` wrapper to produce a complete travel plan.

---

## 📃 Example Prompt

- **Destination**: London, UK
- **Dates**: August 15–22, 2024
- **Budget**: Mid-range (£1000–£1500)
- **Preferences**: Historical sites, local cuisine, avoiding tourist traps

---

## 💻 Running the App

```bash
python llama.py
```

This launches a Gradio UI where you can enter your trip details and generate a customized travel plan.

