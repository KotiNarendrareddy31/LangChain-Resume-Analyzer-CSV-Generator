
# 📄 LangChain-Resume-Analyzer-CSV-Generator

An **LLM-powered resume analysis tool** that takes a **ZIP file containing multiple resumes (PDF/DOCX)** and converts them into a **structured CSV file** using **LangChain**, **Google Gemini**, and **Pydantic schemas**.

This project is ideal for **HR teams, recruiters, and data analysts** who need automated, scalable resume parsing.

---

## ✨ Features

* 📦 Upload a **ZIP file** with multiple resumes
* 📄 Supports **PDF** and **DOCX** formats
* 🤖 AI-powered resume parsing using **Google Gemini**
* 🧱 Strict **schema-based extraction** using Pydantic
* 📊 Automatically generates a **clean CSV**
* 👀 Preview extracted data inside the app
* ⚡ Fast, accurate, and scalable
* 🔐 Secure API key handling with `.env`

---

## 🛠️ Tech Stack

* **Frontend / UI:** Streamlit
* **LLM:** Google Gemini (`gemini-2.5-flash`)
* **AI Framework:** LangChain
* **Schema Validation:** Pydantic
* **File Parsing:** PyPDF2, python-docx
* **Language:** Python

---

## 📂 Project Structure

```
LangChain-Resume-Analyzer-CSV-Generator/
│
├── app.py / notebook.py     # Main Streamlit application
├── .env                     # Google API key (not committed)
├── requirements.txt         # Dependencies
└── README.md                # Documentation
```

---

## 🔑 Prerequisites

* Python **3.9+**
* Google Gemini API key
* Internet connection

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/LangChain-Resume-Analyzer-CSV-Generator.git
cd LangChain-Resume-Analyzer-CSV-Generator
```

---

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

Activate it:

**Windows**

```bat
venv\Scripts\activate
```

**Mac / Linux**

```bash
source venv/bin/activate
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Configure Environment Variables

Create a `.env` file in the project root:

```env
GOOGLE_API_KEY=your_google_gemini_api_key_here
```

⚠️ **Never commit `.env` to GitHub**

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

The app will open automatically in your browser.

---

## 🧠 How It Works

1. Upload a **ZIP file** containing resumes
2. ZIP is extracted to a temporary directory
3. Text is extracted from PDF/DOCX files
4. LangChain sends resume text to **Gemini**
5. Gemini returns structured data following a **Pydantic schema**
6. Data is compiled into a **CSV file**
7. User downloads the CSV instantly

---

## 📊 Extracted Fields (CSV Schema)

* Name
* Email
* Phone
* Skills
* Experience Summary
* Education
* LinkedIn URL
* GitHub URL

---

## 🔐 Security & Privacy

* API key loaded securely from `.env`
* Files processed only in memory / temp directories
* No resume data is permanently stored

---

## 🚀 Use Cases

* 🧑‍💼 HR resume screening
* 📊 Resume data analytics
* 🤖 ATS preprocessing
* 🏫 Campus placement automation
* 📈 Bulk resume structuring

---

## 🚧 Future Enhancements

* Skill-based scoring
* Experience level classification
* Job-role matching
* Multi-language resume support
* Database export (SQL / Excel)
* Resume similarity & deduplication

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 👤 Author

**Narendra Reddy Kotireddy**
🎓 B.Tech CSE (2023)
🎯 Aspiring AI / ML Engineer
🔗 [LinkedIn](https://www.linkedin.com/in/kotireddy-narendra-reddy-5105301a6)

---

