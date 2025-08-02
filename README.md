# DigitalFinancialAdvisor-AI-Agent
PROJECT TITLE
📌 AI Agent for Digital Financial Literacy
Presented by:

Your Name – Aman Kumar Singh

🧾 Problem Statement
Despite the widespread growth of digital finance tools like UPI, many citizens still struggle with understanding how to safely use them. Users are often vulnerable to online fraud, do not understand interest rates or loans, and lack financial literacy. These challenges are more severe in rural and semi-urban areas, where users may also face language barriers.

🧩 Proposed Solution 
We propose an AI-powered multilingual Digital Financial Literacy Agent that:

Answers user questions in their preferred language (e.g., Hindi, Telugu, etc.)

Uses Retrieval-Augmented Generation (RAG) to fetch content from RBI, NPCI, and trusted banking sources

Guides users on safe UPI usage, budgeting, EMI, online scam detection, and personal finance

Uses IBM Granite for natural language understanding and response generation

⚙️ System Development Approach
System Requirements:

    IBM Cloud Lite Account
    
    Python backend (Flask or FastAPI)
    
    IBM Watson Services (Granite, Translator)
    
    Vector database for RAG (Weaviate or compatible)

Libraries:

  flask, ibm-watson, langchain, weaviate-client, openai, transformers

Architecture:

  User sends a query →
  
  Translated to English (if needed) →
  
  Embedded and matched in vector DB (RAG) →
  
  Granite generates answer →
  
  Translated back (if needed) →
  
  Delivered to user (chatbot/voice UI)

🔄 Algorithm & Deployment (Slide 5)
Algorithm Selection:

  Retrieval-Augmented Generation (RAG) using IBM Granite

Input Data:

  User question (e.g., "How do I check if a UPI request is fake?")
  
  Embedded vector database with verified financial documents (e.g., RBI FAQ, NPCI guides)

Training:

  IBM Granite LLM used with pre-processed document chunks
  
  No fine-tuning required due to powerful zero-shot capabilities

Deployment:

  Flask backend deployed on IBM Cloud Lite
  
  IBM Watson used for Language Translation
  
  Frontend as a web app or chatbot interface
  
  IBM Object Storage holds all static PDFs

📸 Result
(Insert a screenshot of the chatbot interface or API response here)

  Example Query:
  "₹500 ka UPI request aaya – fake hai ya genuine?"
  
  Output:
  "Always verify the UPI ID and request source. Don’t approve money requests from unknown senders. Use the BHIM or bank app to check authenticity."

🧾 Conclusion
  The agent makes digital finance safe and understandable for all
  
  Uses IBM Granite to generate accurate, real-time answers
  
  Supports regional languages for inclusiveness
  
  Reduces risks of fraud and builds trust in digital transactions

🔭 Future Scope
  WhatsApp and Voice integration for elderly users
  
  Real-time scam alerting using NLP-based detection
  
  Step-by-step voice instructions for actions like UPI transfers
  
  Personalized modules for students, workers, and senior citizens

📚 References
  https://www.rbi.org.in
  
  https://www.npci.org.in

  https://www.financialliteracy.gov.in

IBM Granite and Watsonx.ai documentation

LangChain, Weaviate for RAG
