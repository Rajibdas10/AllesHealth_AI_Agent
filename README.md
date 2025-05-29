# AllesHealth_AI_Agent
AllesHealth AI is a prototype AI-powered assistant designed to help hospital staff and billing teams answer reimbursement-related questions using natural language. 

Here’s a professional and concise `README.md` content tailored for your GitHub project:

---

# 💡 AllesHealth AI Agent – Reimbursement Query Assistant

An AI-powered assistant prototype that helps hospital staff quickly find reimbursement information using natural language queries. This tool intelligently parses structured medical tariff data (ICD/OPCS codes) and provides relevant answers using vector search and language models.

## 📌 Project Overview

**Use Case**: Hospital staff often need to check reimbursement codes, procedure costs, and diagnostic details. This assistant automates that task through an intuitive QA interface.

**Sample Queries Supported**:

* "What is the reimbursement for a knee replacement surgery?"
* "Is there a different rate for out-patient dialysis?"
* "How much does insurance cover for procedure code 10293?"
* "What’s the code for Brain Tumours or Cerebral Cysts, with CC Score 2-3?"

## ⚙️ Features

* 🧠 Natural Language Understanding (NLU)
* 🔍 Knowledge Retrieval using FAISS vector search
* 📄 Support for ICD-10 and OPCS datasets
* 🤖 Mistral-7B integration via OpenRouter API
* 🖥️ CLI-based QA Interface (Web interface coming soon!)

## 🛠️ Tech Stack

* Python
* Pandas
* LangChain
* SentenceTransformers (MiniLM-L6-v2)
* FAISS (Vector DB)
* Mistral-7B (via OpenRouter API)

## 📂 Project Structure

```bash
.
├── ICD_10_Codes_Jan2025.xlsx           # ICD-10 data (diagnostic codes)
├── OPCS_code_analysis.xlsx            # OPCS codes (procedure codes)
├── alleshealth_ai_agent.ipynb         # Main notebook (core logic)
├── assets/                            # Screenshots, visuals, sample queries
└── README.md                          # Project documentation
```

## 🚀 How It Works

1. **Load & Merge ICD and OPCS data**
2. **Generate embeddings** using MiniLM
3. **Store vectors in FAISS**
4. **Connect to Mistral-7B** using OpenRouter
5. **Answer natural language queries** using LangChain RetrievalQA

## ✅ Setup Instructions

```bash
# Clone the repository
git clone https://github.com/yourusername/AllesHealth_AI_by_RajibDas.git
cd AllesHealth_AI_by_RajibDas

# Install requirements
pip install -r requirements.txt
```

## 🔑 API Setup

Set your OpenRouter API Key:

```python
os.environ["OPENROUTER_API_KEY"] = "your-key-here"
```

## 🧪 Sample Output

<img src="assets/sample_query_output.png" width="600"/>

## 📈 Future Enhancements

* ✅ Web-based interface
* 🔒 Secure user authentication
* 🧾 Billing integration for hospitals
* 🗂️ Historical query logs

---

## 🤝 Contributing

We welcome contributions! Please open issues or pull requests.

---

## 📬 Contact

**Author**: Rajib Das

