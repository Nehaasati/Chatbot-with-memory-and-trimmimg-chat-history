Chatbot_using_Langchain_with_Memory (Groq + Gemma 2)
This Colab notebook demonstrates a chatbot I built using LangChain and Gemma 2 via the Groq API. The implementation showcases key LangChain features such as memory handling, prompt templating, and message trimming to manage token usage effectively.

🚀 Key Features
Groq API Integration (Gemma 2):
Uses the Gemma 2 model served via the Groq API for fast and intelligent natural language responses.

Chat Memory with Context Preservation:
Implements InMemoryChatMessageHistory to store previous messages and retain context across multiple user inputs.

Multiple Chat Sessions:
Supports multiple independent sessions, each maintaining its own history and conversation flow.

Prompt Templates:
Uses ChatPromptTemplate for structured and consistent message formatting, improving response quality.

Message Trimming Technique:
Applies trim_messages to control the context window and avoid exceeding token limits—ensuring efficient and scalable conversations.

Runnable Chains with Memory:
Combines the prompt template, LLM model (Gemma 2 via Groq), and memory into a clean, modular Runnable chain, streamlining the chatbot logic.

📦 Setup and Dependencies
The notebook installs and uses:

langchain

langchain_community

langchain_google_genai (optional, not used here with Groq)

You’ll also need to set the necessary environment variables for API access and optional LangChain tracing.

🔑 Environment Variables
Before running the notebook, make sure to set the following:

GROQ_API_KEY – Your Groq API key to access Gemma 2.

LANGCHAIN_API_KEY – Your LangChain API key.

LANGCHAIN_TRACING_V2, LANGCHAIN_PROJECT, LANGCHAIN_ENDPOINT – For LangChain tracing (optional).

TAVILY_API_KEY – For search tool integration (optional).

HUGGINGFACEHUB_API_TOKEN – For additional model/tool use (optional).

⚠️ Important: Replace any placeholder keys with your actual credentials before running.

🧠 Usage
Open the notebook in Google Colab.

Replace placeholder API keys with your own.

Run all cells to initialize the chatbot.

The chatbot starts with a welcome message and runs in a loop until you type "bye".

🧪 Demonstrated Examples
Basic Chat using Gemma 2 from Groq.

Chat Memory: Maintains history using InMemoryChatMessageHistory.

Multiple Sessions: Each session has its own isolated memory.

Prompt Templates: Clean formatting for model prompts.

Token Trimming: Demonstrates trimming old messages to fit within the context window.

Chained Interaction: Using Runnable chains that integrate all parts into one coherent flow
