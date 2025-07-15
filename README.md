# 📊 Trade Opportunities API

This FastAPI service analyzes current news and trends in Indian market sectors to generate trade opportunity reports in Markdown format.

---

## 🚀 Features

- ✅ Analyze sectors like farming, pharmaceuticals, tech, etc.
- ✅ Returns Markdown report ready to be saved as `.md`
- ✅ Real-time market news collection
- ✅ Gemini based LLM-based analysis
- ✅ Rate limiting & security controls
- ✅ API documentation via Swagger

---

## 📦 Setup Instructions

1. Clone the Repo
✅git clone https://github.com/yourname/trade-opportunity-api.git
✅cd trade-opportunity-api
2. Create Virtual Environment
-> python -m venv env
-> source env/bin/activate 
3. Install Dependencies
-> pip install -r requirements.txt
5. Run the API
6. uvicorn main:app --reload
   
## 📘 API Reference
GET /analyze/{sector}
-> Returns a structured markdown report for the given sector.
Example:
GET /analyze/farming

-> Response:
{
  "sector": "farming",
  "report": "# Market Analysis Report: Farming\n\n## Summary\n..."
}
## 🔐 Security
Token-based (HTTPBearer) authentication (optional)
Rate limiting per user/session
Input validation and error handling

✅ Project Folder Structure
trade-opportunities-api/
│
├── main.py
├── requirements.txt
├── README.md
├── .env                  # (Optional: your API keys)
│
├── auth.py
├── limiter.py
├── collector.py
├── analyzer.py
├── models.py
├── utils.py
│
├── reports/              # Markdown files are saved here
│
└── __init__.py




