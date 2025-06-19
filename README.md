# DocuSense

DocuSense – Q&A Retrieval System
DocuSense is an AI-powered document-based Question & Answer system that enables users to upload documents (PDFs) and ask natural language questions. It uses semantic search to retrieve relevant chunks from the documents and generates accurate answers using a language model.

🔍 Features

1. Upload and parse documents (PDF format)
2. Generate dense embeddings using SentenceTransformers
3. Perform fast and accurate similarity search using FAISS
4. Retrieve the most relevant document segments based on user queries
5. Generate context-aware answers using a pre-trained transformer model
6. Real-time question answering interface using Gradio

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
git clone https://github.com/YASH212414/DocuSense.git
cd DocuSense-

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
