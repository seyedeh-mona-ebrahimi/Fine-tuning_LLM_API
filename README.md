# Fine-tuning_LLM_API

# 🎭 Sentiment Analysis App  

A complete **Sentiment Analysis** application with a **FastAPI backend**, **React frontend (Vite + Tailwind)**, and a **Jupyter Notebook** for model training.

---

## 📌 Features
✔️ Analyze sentiment using **Llama 3** and **My Custom Model ('SeyedehMonaEbrahimi/fine-tuned-imdb')**  
✔️ Provides **sentiment** (positive/negative) and **confidence score**  
✔️ Backend API built with **FastAPI**  
✔️ Frontend using **React (Vite) + Tailwind CSS**  
✔️ Jupyter Notebook for training/testing models  
✔️ Three ways to test API: Python script, `curl`, and Postman**  

---

## 🚀 Installation & Setup  

### 1️⃣ Clone the Repository  
```sh
git clone https://github.com/YOUR_GITHUB_USERNAME/sentiment-analysis.git
cd sentiment-analysis



### 2️⃣ Running the Jupyter Notebook
📌 Location: notebook/sentiment_analysis.ipynb

Install dependencies (if not already installed):
```sh
pip install -r backend/requirements.txt
Start Jupyter Notebook:
```sh
jupyter notebook

Open sentiment_analysis.ipynb and run all cells.





## 3️⃣ Running the Backend (FastAPI)
📌 Location: backend/app.py

Navigate to the backend folder:
```sh
cd backend
Install dependencies:
```sh
pip install -r requirements.txt
Start the FastAPI server:
```sh
uvicorn app:app --reload



API will be available at:
Docs: http://127.0.0.1:8000/docs
Analyze Sentiment: http://127.0.0.1:8000/analyze




🎨 4️⃣ Running the Frontend (React + TailwindCSS)
📌 Location: sentiment-ui/

Navigate to the UI folder:
cd sentiment-ui
npm run dev
