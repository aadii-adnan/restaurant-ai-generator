# restaurant-ai-generator
🍴 AI Restaurant Concept & Menu Generator
An intelligent multi-stage LLM application that generates a unique restaurant brand and a curated menu based on a selected cuisine.

### 🚀 Try it Out
* **Live Notebook:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aadii-adnan/restaurant-ai-generator/blob/main/Menu_Gen.ipynb)

🛠️ Tech Stack
Framework: LangChain (LCEL - LangChain Expression Language)

AI Model: Llama 3.3 via Groq LPU (Language Processing Unit) for near-instant response times

Frontend: Streamlit

Language: Python

💡 Technical Logic (How it Works)
This project moves beyond simple "one-off" prompts by implementing a Sequential Chain. This allows the AI to maintain context across different tasks.

Station 1 (Branding): Takes a user-defined cuisine and generates a sophisticated restaurant name using a dedicated PromptTemplate.

The Handover (LCEL): Using the Pipe Operator (|) and RunnablePassthrough, the output of the first stage is automatically injected into the second stage.

Station 2 (Menu Generation): Uses the generated name to create a matching, thematic menu list.

📂 Repository Structure
app.py: The main Streamlit web application code.

Menu_Gen.ipynb: The original development notebook showing the logic experiments.

requirements.txt: List of dependencies needed to run the project.

⚙️ Setup Instructions
Clone the repo: git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME.git

Install dependencies: pip install -r requirements.txt

Set your API Key: Add your Groq API key to your environment variables as GROQ_API_KEY.

Run the app: streamlit run app.py
