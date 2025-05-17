# 🤖 Q&A AI Agent with RAG using n8n (Free Setup)

Build your own smart **AI chatbot** that can answer questions using its **own knowledge base** — powered by **Google Gemini**, **Pinecone**, and **n8n** — all without writing any code!

---

## 🔍 Features

- 💬 Chatbot built using **n8n AI Agent**
- 🧠 Uses **Google Gemini embeddings + language model**
- 📂 Pulls content from **Google Drive**
- 🔗 Stores data in **Pinecone vector database**
- 🧠 Equipped with **Simple Memory** for better context awareness
- 📚 Uses **Retrieval-Augmented Generation (RAG)** to answer from your own documents
- ✅ Fully customizable and open-source setup

---

## 🧰 Tech Stack

- [n8n](https://n8n.io) – Automation platform (self-hosted or cloud)
- [Google Gemini](https://deepmind.google) – For embeddings + chat model
- [Pinecone](https://www.pinecone.io/) – Vector database for long-term knowledge
- Google Drive – Source of the knowledge documents (PDFs, etc.)

---

## 🚀 How It Works

1. 📂 **Upload a PDF or document** to your Google Drive.
2. 🔄 n8n workflow fetches the file using **Google Drive node**.
3. 🧠 The document is split into chunks using the **Recursive Character Text Splitter**.
4. 🧬 Each chunk is embedded using **Google Gemini Embeddings**.
5. 📥 Embedded vectors are stored in **Pinecone** under a specific namespace.
6. 💬 When a chat message is received, the **AI Agent**:
   - Uses **Simple Memory** for context.
   - Queries the **Pinecone Vector Store**.
   - Retrieves the most relevant chunks.
   - Uses **Gemini Chat Model** to generate an accurate, contextual response.

---

## 🧪 Sample Use Case

> User: "Who is Anaam?"
>
> Agent: "Anaam Rasool is the founder and CTO of Fast AI agency. With a background in software engineering and strong public speaking skills, he's a driving force behind the company."

---

## 🛠 Setup Instructions

1. Clone or import the workflow in your n8n instance.
2. Set up the following credentials:
   - Google Drive OAuth
   - Google Gemini API
   - Pinecone API
3. Upload your document to Google Drive.
4. Modify the file ID in the **Google Drive node** if needed.
5. Activate the workflow.
6. Interact with your chatbot via the **Chat Trigger node** or webhook.

---

## 🧠 System Prompt Used

The agent uses a refined system prompt to interpret responses returned from vector tools naturally, without repeating them robotically. It answers like a human, maintaining context and flow.

---

## 📎 Related Links

- [n8n Docs](https://docs.n8n.io)
- [Pinecone Docs](https://docs.pinecone.io)
- [Google Gemini API](https://makersuite.google.com/)

---

## 🏷️ Tags

`n8n` `AI Agent` `RAG` `Gemini` `Pinecone` `chatbot` `no-code` `AI automation` `vector db` `knowledge base chatbot`

---

## 📜 License

This project is open-source and available under the MIT License.

---

> Built with ❤️ using n8n and AI.
