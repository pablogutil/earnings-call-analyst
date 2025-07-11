# AI Earnings Call Analyst 🎧📊

A smart LLM-powered tool that parses, analyzes, and summarizes earnings call transcripts.

---

## 📊 What It Does

- 📄 **Transcript Ingestion**  
  Scrapes calls from SeekingAlpha or uploads your own `.txt` file

- 🧠 **Sentiment Analysis**  
  FinBERT assigns scores to each section or speaker

- 🔍 **Theme Detection**  
  LLM detects dominant business topics (e.g. “cost control”, “China demand”)

- 🐂🐻 **Bull/Bear Summary**  
  GPT-4 generates an investor-focused takeaway

---

## 🛠 Stack

- **Backend:** FastAPI  
- **Frontend:** Next.js (Tailwind, React)  
- **NLP:** FinBERT (HuggingFace) + GPT-4  
- **Optional:** Supabase for auth + transcript storage

---

## 📸 Example Output

> **Apple Q2 2024:**  
> - 73% Positive Sentiment (↑12% YoY)  
> - 🔑 Top Themes: China Demand, Cost Restructuring  
> - 📉 Bearish: iPhone upgrade cycle softness

---

## 🤖 Why It Matters

Wall Street analysts pay thousands for tools like this.  
This repo is your way to build it **yourself**, open-source and modular.

---

## 🧪 Try It

```bash
# Ingest transcript
POST /analyze-call  
{
  "url": "https://seekingalpha.com/..."
}
