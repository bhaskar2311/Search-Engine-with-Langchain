# 🔍 AI-Powered Search Engine using Langchain & Groq

A fully interactive end-to-end search engine chatbot built with Langchain and powered by Groq’s ultra-fast LLaMA3 model. This app enables natural language queries and searches across Wikipedia, Arxiv, and DuckDuckGo to return rich, multi-source answers — all within a user-friendly Streamlit interface.

## 📌 Features
* 🧠 Ask any question and receive consolidated answers from multiple search tools
* 🌐 Integrates Wikipedia, Arxiv, and DuckDuckGoSearch for comprehensive results
* ⚡ Built on Groq’s LLaMA3-8B-8192 for fast and fluent response generation
* 💬 Chat-style interface with conversation history retention using Streamlit
* 🔧 Uses Langchain’s tool-agent framework (ZERO_SHOT_REACT_DESCRIPTION)

## 🧠 Technologies Used
* Streamlit – For building the chat-based UI
* Langchain – Tool invocation, agent orchestration
* Groq API – LLaMA3-8B for fast response inference
* WikipediaAPIWrapper – For structured wiki search
* ArxivAPIWrapper – Academic paper search integration
* DuckDuckGoSearch – Web-wide keyword search
* dotenv – Secure API key management

## 🗂 Project Structure
```
├── app.py                  # Main Streamlit app
├── tools_agent.ipynb       # Agent test script / prototype
├── requirements.txt        # Python dependencies
└── .env                    # API keys (excluded from repo)
```

## ⚙️ Setup Instructions
1. Clone the Repository
```
git clone https://github.com/bhaskar2311/Search-Engine-with-Langchain
cd Search-Engine-with-Langchain
```
2. Create a Virtual Environment (optional but recommended)
```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3. Install Dependencies
```
pip install -r requirements.txt
```
4. Setup Environment Variables
  * Create a .env file in the root directory and add your API keys like this:
```
# .env
GROQ_API_KEY=your_groq_key_here
```
🚨 Warning: Never commit .env files to public repositories.

## 🚀 How to Run
```
streamlit run app.py
```
* Enter your Groq API Key in the sidebar.
* Type a natural language query (e.g., What is machine learning?)
* Watch the assistant search across Wikipedia, Arxiv, and the web in real-time.
* Get a clear, final answer with source summaries below.

## 📦 Reusability
* This application is designed to be easily extended:

  - You can extend this project to include additional data sources like YouTube, StackOverflow, or news APIs.

  - The tools_agent.ipynb file contains testing/integration logic used for rapid prototyping.

 ## 📸 Screenshots
 ![Output](https://github.com/user-attachments/assets/54c93efd-1c1f-4b18-99b5-bdb4a5a9aef2)

 ## 📝 Notes
This project was fully developed by me. The README was written based on my knowledge and experience, with support from generative AI tools to refine its structure and presentation.

## 📄 License
This project is open source and available under the MIT License.

## 🙋‍♂️ Author
Made with ❤️ by Bhaskar Shivaji Kumbhar
