# ✈️ AI Travel Planner — Advanced GenAI Version

An AI-powered travel planning project that generates personalized itineraries based on destination, travel dates, budget, interests, and preferences. Built with Python and Generative AI, the project demonstrates LLM integration, structured itinerary generation, budget allocation, and automated itinerary validation.

> **Disclaimer:** This is a portfolio and learning project, not a live booking service. Prices, opening hours, weather, transport schedules, availability, and visa requirements are not verified. Confirm important information through official sources before traveling.

## ✨ Features

- 🤖 **GenAI Itinerary Generation** — Generate structured travel plans using an OpenAI-compatible LLM API.
- 🧭 **Personalized Travel Planning** — Customize trips using dates, destinations, interests, and travel styles.
- 💰 **Budget Allocation** — Estimate spending across accommodation, food, transport, activities, and contingency.
- 🎯 **Interest-Based Recommendations** — Rank activities according to user preferences.
- ✅ **Itinerary Validation** — Check date coverage, activity duration, and budget allocations.
- 🔄 **Fallback Planning** — Run a demonstration itinerary without an API key.
- 📤 **Export Support** — Export travel plans in JSON and Markdown formats.
- 🔐 **Environment-Based Configuration** — Keep API credentials outside the source code.

## 🛠️ Tech Stack

- Python
- Jupyter Notebook
- Pandas
- Generative AI and Large Language Models
- OpenAI-compatible API
- Python-dotenv
- JSON

## 📂 Project Structure

```text
ai-travel-planner-advanced-genai/
│
├── ai_travel_planner_advanced_genai.ipynb
├── README.md
├── requirements.txt
├── .env.example
└── .gitignore
```

## 🚀 Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/ai-travel-planner-advanced-genai.git
cd ai-travel-planner-advanced-genai
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Create a virtual environment

**Windows PowerShell**

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

**macOS/Linux**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the LLM API (Optional)

Copy `.env.example` to `.env` and configure the credentials for your chosen OpenAI-compatible provider.

```env
OPENAI_API_KEY=your_api_key_here
OPENAI_BASE_URL=
OPENAI_MODEL=gpt-4.1-mini
```

- `OPENAI_API_KEY`: API key for the selected provider.
- `OPENAI_BASE_URL`: Optional provider-specific API endpoint.
- `OPENAI_MODEL`: Model name supported by your provider.

**Security:** Never upload your actual API key or `.env` file to GitHub.

The notebook can use its demonstration fallback when an API key is unavailable.

### 5. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
ai_travel_planner_advanced_genai.ipynb
```

Run the notebook cells from top to bottom.

## 🧠 How It Works

1. Enter the destination, dates, budget, and traveler preferences.
2. Convert the trip request into a structured prompt.
3. Generate an itinerary through an LLM or the fallback planner.
4. Display planned activities in a table.
5. Validate dates, activity durations, and budget allocations.
6. Rank activities based on user interests.
7. Export the generated plan as JSON and Markdown files.

## 📊 Example Use Case

A traveler wants to visit Jaipur, Rajasthan, for four days with a budget of ₹25,000 for two people.

The planner accepts the travel dates, budget, interests such as history and architecture, and preferences such as vegetarian food options. It then generates a sample itinerary and budget breakdown.

The example is intended to demonstrate the workflow. It does not represent verified prices or a confirmed itinerary.

## ⚠️ Current Limitations

- The fallback itinerary is generic and is not verified for a specific destination.
- Budget allocations are illustrative estimates, not live quotes.
- Live maps, weather, booking, ticket availability, and visa services are not integrated.
- Structural validation cannot guarantee factual accuracy.
- Interest matching uses simple keyword rules rather than semantic embeddings.
- The notebook is a prototype, not a production-ready travel service.

## 🔮 Future Enhancements

- Integrate a maps and places API.
- Add live weather and time-zone information.
- Implement Retrieval-Augmented Generation (RAG) using trusted travel guides.
- Add source links for destination information.
- Build a Streamlit or React user interface.
- Add user accounts and saved itineraries.
- Add route optimization and travel-time estimation.
- Add automated tests, retries, rate limiting, and prompt-injection defenses.
- Add multilingual itinerary generation.

## 🔐 Responsible AI and Security

- Verify travel details with official sources before booking.
- Do not send passport numbers, payment details, or other sensitive personal information to an LLM.
- Keep API keys in environment variables.
- Treat generated recommendations as suggestions, not guarantees.

## 📄 License

Choose a license, such as MIT, before publishing the repository, and add the corresponding `LICENSE` file.

---

**Built with Python, Jupyter Notebook, Pandas, and Generative AI.**
