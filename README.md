# DocuSense
DocuSense – Q&A Retrieval System
DocuSense is an AI-powered document-based Question & Answer system that enables users to upload documents (PDFs) and ask natural language questions. It uses semantic search to retrieve relevant chunks from the documents and generates accurate answers using a language model.

🔍 Features
Upload and parse documents (PDF format)

Generate dense embeddings using SentenceTransformers

Perform fast and accurate similarity search using FAISS

Retrieve the most relevant document segments based on user queries

Generate context-aware answers using a pre-trained transformer model

Real-time question answering interface using Gradio

🛠 Tech Stack
Component	Tech Used
Embedding Model	SentenceTransformers (MiniLM-L6-v2)
Vector Store	FAISS (Facebook AI Similarity Search)
Document Parsing	PyMuPDF (fitz)
Answer Generation	Hugging Face Transformers (LLMs)
Frontend UI	Gradio
Programming Language	Python

📂 Project Structure
DocuSense/
├── docs/                   # Sample PDFs or test files
├── utils.py                # Document parsing & chunking utilities
├── app.py                  # Main Gradio interface
└── requirements.txt        # Python dependencies

🚀 How to Run Locally
1. Clone the Repository
git clone https://github.com/YeshwanthMotivity/DocuSense-.git
cd DocuSense-/project/Q-A_Retrieval

2. Install Dependencies
pip install -r requirements.txt

3. Run the App
python app.py
Gradio will launch a local server in your browser. Upload a document and start asking questions!

🧠 How It Works
1. Document Upload: User uploads a PDF file.

2. Text Extraction: The PDF is parsed and split into logical chunks.

3. Embedding & Indexing: Each chunk is embedded and stored in a FAISS index.

4. Query Handling: User inputs a question → converted to embedding → nearest relevant chunks retrieved.

5. Answer Generation: A pre-trained LLM is used to generate a natural response based on the retrieved content.

📈 Future Improvements
1. Support DOCX and TXT files

2. Add context memory across multi-turn conversations

3. Allow saving and reusing indexed documents

4. Deploy on cloud (Hugging Face Spaces / Streamlit Cloud)

📬 Contact
For suggestions, improvements, or questions:
📧 mudimalayeshwanthgoud@gmail.com
