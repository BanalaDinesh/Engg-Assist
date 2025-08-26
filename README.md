# 🎓 Engg Assist - Hyderabad B.Tech Chatbot 🤖

A **Colab-based chatbot** built using **LangChain + FAISS + Gradio + Ollama**.  
It helps students explore **Hyderabad engineering colleges** with details like:

- ✅ Fees  
- ✅ Cutoffs  
- ✅ Placements  
- ✅ Accreditations  
- ✅ Courses offered  

---

## 🚀 Features
- Retrieval-Augmented Generation (RAG) pipeline using **FAISS Vector DB**
- Hybrid embedding support (**Ollama** + **HuggingFace** fallback)
- Natural, conversational answers
- Gradio-based UI for chatting
- Preloaded Hyderabad colleges dataset + FAQs

---

## 📂 Project Structure  

chatbot/  
├── hyderabad_engineering_colleges.csv  
├── hyd_college_faq_extended.csv  
│── engg_assist_colab.ipynb # Main Google Colab notebook  
├── README.md # Documentation   


---

## ⚙️ Installation & Usage

### 1️⃣ Open in Google Colab  
Click below to launch directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BanalaDinesh/chatbot/blob/main/notebook/Enggassist.ipynb)

---

### 2️⃣ Upload Required CSVs  
Inside Colab, upload your CSV files:  

- `hyderabad_engineering_colleges.csv`  
- `hyd_college_faq_extended.csv`

---

### 3️⃣ Run the Notebook  
Run all cells in `engg_assist_colab.ipynb`.  
This will:
- Install dependencies
- Start **Ollama server** inside Colab
- Pull LLaMA and embedding models
- Build FAISS vector index
- Launch Gradio Chatbot (with `share=True` for public link)

---

## 📊 Data Sources
- `hyderabad_engineering_colleges.csv` → College details (fees, branches, cutoffs, etc.)  
- `hyd_college_faq_extended.csv` → FAQs with predefined answers  

---

## 🛠️ Requirements
Even though Colab handles installs, here are dependencies for clarity:

```txt
langchain
langchain-community
faiss-cpu
sentence-transformers
gradio
pandas
nltk
