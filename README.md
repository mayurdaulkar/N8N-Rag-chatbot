🤖 RAG Chatbot for Internship Q&A (n8n + Pinecone + Gemini)

This is a no-code AI chatbot that answers questions based on your internship report — built fully in n8n using Gemini, Pinecone, and Google Drive.

---

## 💼 What's Inside?

| File | What it does |
|------|---------------|
| `Data_Feeding.json` | Pulls internship report from Google Drive, splits it, turns it into embeddings, and stores in Pinecone |
| `RAG_CHATBOT.json`  | Chatbot that uses AI to answer questions based on that data |

---

🛠️ Tech Used

- 🔄 n8n (workflow automation)
- 📁 Google Drive (file source)
- 🧠 Gemini API (embeddings + answers)
- 📦 Pinecone (vector search DB)

---

⚙️ How It Works (In Simple Words)

1. Your internship PDF is on Google Drive.
2. First workflow reads it, chunks it, turns it into vectors using Gemini, and sends it to Pinecone.
3. Second workflow is your chatbot.
4. It takes your question, finds the best matching chunks from Pinecone, and uses Gemini to answer.

---

🚀 How to Use

1. Import both workflows in n8n
2. Add your:
   - Pinecone API key
   - Gemini API key
   - Google Drive credentials
3. Run the **data feeding** workflow once.
4. Start the **chatbot** and ask anything 🔥

---

💬 Example

**You:** "What did I learn in my internship?"  
**Bot:** "Based on your report, you learned about machine learning, data cleaning, and automation tools."

---


