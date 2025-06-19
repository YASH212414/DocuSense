DocuSense – Document-Based Q&A Retrieval System

DocuSense is an intelligent document question-answering system that allows users to upload a document (PDF format), ask natural language questions, and receive context-aware answers. It leverages semantic search techniques and large language models to extract relevant information from unstructured documents.

Features

1. Upload PDF documents for intelligent reading

2.  Semantic search powered by SentenceTransformers and FAISS

3.  AI-generated answers using Hugging Face Transformers

4.  Interactive Q&A UI built with React.js

5.  Flask backend to serve LLM responses and handle embedding logic

🛠️ Tech Stack

1. Layer	Tools Used
2. Frontend	React.js, HTML, CSS
3. Backend	Flask (Python), PyMuPDF (fitz), Transformers
4. NLP Models	SentenceTransformers (MiniLM), Hugging Face LLMs
5. Search	FAISS – Fast Approximate Nearest Neighbor Search
6. Deployment	Flask API, local server (extendable to Render/Heroku)

🧾 Project Workflow

1. Document Upload: User uploads a PDF through the React UI.

2. Text Extraction: Flask backend parses and chunks the PDF using PyMuPDF.

3. Embedding: Each chunk is vectorized using a SentenceTransformer.

4. Semantic Search: On question input, relevant chunks are retrieved via FAISS.

5. Answer Generation: LLM uses the question and relevant context to generate an accurate answer.

6. Response: The answer is sent back to the frontend and displayed in real time.

📂 Folder Structure

DocuSense/
├── backend/                      # Flask backend logic
│   ├── app.py                    # Main Flask app
│   ├── embedding_utils.py        # FAISS + model logic
│   └── requirements.txt          # Python dependencies
├── frontend/                     # React frontend
│   ├── src/
│   │   └── components/
│   │       └── UploadForm.js     # File upload and Q&A UI
│   └── package.json
└── README.md

💻 Running Locally

🧩 Backend (Flask)

cd backend

pip install -r requirements.txt

python app.py

🌐 Frontend (React)

cd frontend

npm install

npm start


🎯 Future Improvements

1. Support for DOCX and TXT formats

2. Upload multiple documents and maintain context history

3. Add authentication for private document handling

4. Dockerize for seamless deployment

🤝 Contact
For suggestions or collaboration opportunities, feel free to reach out:

📧 mudimalayeshwanthgoud@gmail.com
