# 🧠✈️ Multi-Agent Trip Planner

An intelligent, AI-powered travel planner built with **Streamlit**, **CrewAI**, **Groq LLaMA3**, and **SerpAPI**. This app uses multiple autonomous agents to generate personalized flight options, hotel recommendations, and a detailed day-wise travel itinerary based on your preferences.

---

## 🔧 Features

- ✈️ **Flight Suggestions:** Real-time flight info fetched via Google Flights (SerpAPI).
- 🏨 **Hotel Finder:** Budget-based hotel listings using live hotel data.
- 🗓️ **AI Itinerary Planner:** Personalized daily travel plan using LLM-based agents.
- ✍️ **Interactive Itinerary Editing:** Users can change any part of the plan by chatting naturally.

---

## 🧠 Powered By

- **LLM**: `llama3-70b-8192` via **Groq API**
- **Agent Framework**: [CrewAI](https://docs.crewai.com/)
- **Live Data**: [SerpAPI](https://serpapi.com/) for Flights and Hotels
- **Frontend**: [Streamlit](https://streamlit.io/)

---

## 🚀 How It Works

1. User answers 4 questions:
   - Where would you like to travel?
   - How many days will your trip be?
   - What's your budget? (low-range, mid-range, luxury)
   - Which city will you depart from?

2. System Actions:
   - Fetches live flights and hotels from SerpAPI
   - Uses CrewAI agents to summarize options
   - Creates a multi-day itinerary using LLMs

3. ✅ **After generation**, you can edit it using plain English prompts like:
   - Change Day 2 Morning to visit Eiffel Tower
   - Replace Day 4 Evening with a beach party
   - Remove Day 5 Afternoon activity
  
4. The **Itinerary Editor Agent** understands the context and applies updates without affecting the rest of the plan.

---

## 🛠️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/multi-agent-trip-planner.git
cd multi-agent-trip-planner
