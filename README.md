📚 Book RAG
Book RAG is a modern Retrieval-Augmented Generation (RAG) application for interactive question-answering over PDFs and documents. Users can upload books, organize them into libraries, ask questions, and revisit past conversations — all powered by a fast backend and sleek frontend.

🚀 Features
📁 Library & PDF Management
Organize multiple libraries and upload PDFs with ease.

💬 Chat Interface
Ask context-aware questions about your documents and receive precise answers.

🕘 Conversation History
View and continue previous chat sessions, grouped by library.

🔍 RAG Pipeline
Combines vector + keyword retrieval for accurate answers.

🖥️ Modern UI
Responsive React + Tailwind interface with dark mode.

📖 Book Branding
Custom favicon and themed branding for a polished experience.

🧰 Tech Stack
Layer	Tech
Frontend	React, Vite, TypeScript, Tailwind CSS, Radix UI, Lucide Icons
Backend	FastAPI, SQLAlchemy, FAISS, HuggingFace Transformers
Database	SQLite (default, easily swappable)
Vector Store	FAISS
LLM	Local (via Ollama) or any HuggingFace-compatible model

⚙️ Getting Started
📌 Prerequisites
Python 3.10+

Node.js 18+

(Optional) Ollama or HuggingFace model for local LLM inference

🖥️ Backend Setup
bash
Copy
Edit
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn backend.main:app --reload
Backend runs at: http://localhost:8000

🌐 Frontend Setup
bash
Copy
Edit
cd frontend
npm install
npm run dev
Frontend runs at: http://localhost:5173

🧪 Usage
📤 Upload PDFs into a chosen library.

❓ Ask questions in the Chat tab.

🕘 Continue previous conversations in the History tab.

🔄 Switch libraries via sidebar or dropdown.

🗂️ Project Structure
csharp
Copy
Edit
book-rag/
├── backend/
│   ├── main.py                # FastAPI entrypoint
│   ├── requirements.txt       # Backend dependencies
│   ├── database/              # SQLAlchemy models and DB logic
│   ├── routes/                # API endpoints
│   ├── services/
│   │   └── rag_pipeline.py    # RAG logic
│   ├── vector_store.py        # FAISS interaction
│   ├── uploaded_pdfs/         # Stored PDFs
│   └── vector_chunks/         # Embedded PDF chunks
├── frontend/
│   ├── src/                   # React source code
│   ├── public/                # Static assets (icons, favicon)
│   ├── index.html             # Entry HTML
│   └── package.json           # Frontend config
🎨 Customization
Branding / Favicon
Replace frontend/public/book-favicon-v2.png and update index.html.

Language Model
Modify backend/services/rag_pipeline.py to change or enhance the LLM.

📄 License
This project is licensed under the MIT License.
See the LICENSE file for details.

🙏 Acknowledgements
Thanks to the amazing open-source ecosystem:

FastAPI

React

Vite

Tailwind CSS

FAISS

HuggingFace Transformers

Ollama

Radix UI

Lucide Icons

🤝 Contributing
Feel free to open an issue or submit a pull request.
We welcome contributions of any kind!

