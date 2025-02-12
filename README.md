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
cd backend

Install dependencies:
pip install -r requirements.txt

Start the FastAPI server:
uvicorn app:app --reload

API will be available at:
Docs: http://127.0.0.1:8000/docs
Analyze Sentiment: http://127.0.0.1:8000/analyze




---------------------------------------------------------------------------

🎨 4️⃣ Running the Frontend (React + TailwindCSS)
📌 Location: sentiment-ui/

Navigate to the UI folder:
cd sentiment-ui
npm run dev







📡 5️⃣ API Usage (Testing in 3 Ways)
➡️ Method 1: Using Python (test_api.py)
📌 Location: backend/test_api.py

Run the API server first:

uvicorn app:app --reload


Run the test script:

python test_api.py


-------------------------------------------------------------------

➡️ Method 2: Using curl (Command Line)
After running uvicorn app:app --reload, test using curl:

curl -X 'POST' 'http://127.0.0.1:8000/analyze/' \
-H 'Content-Type: application/json' \
-d '{"text": "I love this!", "model": "custom"}'

-------------------------------------------------------------------

➡️ Method 3: Using Postman
Open Postman
Enter the API URL:
http://127.0.0.1:8000/analyze/

Choose POST method
Go to "Body" → Select "raw" → Choose JSON format

Enter this JSON payload:
json
{
    "text": "I love this!",
    "model": "custom"
}

Click "Send" and check the response


--------------------------------------------------------------------

🔄 6️⃣ Change Sentences & Models Anytime
Modify the text in the Python script, curl, or Postman.
Change the model between "custom" and "llama" in all three methods.
