# VTUHub — 1BAIA103 Introduction to Artificial Intelligence

Self-learning web application for **Visvesvaraya Technological University** course **1BAIA103: Introduction to Artificial Intelligence and its Applications**, Module 1 (Part A).

## What you can do

- Read **classroom notes** rewritten in Indian English with figures, formulae and tables, **cited** to the prescribed textbook so that you do not copy verbatim.
- Practise **VTU-style SEE/CIE questions** (2 marks, 5–6 marks, 8–10 marks).
- **Type your answer**; the app compares it with the model notes, scores concept coverage and **suggests** which notes, slides or video lecture to revise.
- Watch a **classroom slide deck** and a **video-style lecture** (slides + spoken narration in the browser).

## Academic honesty / citations

All figures, tables and formulae are **redrawn** from the Module 1 textbook (the attached *Introduction to Artificial Intelligence* notes). Running text is **paraphrased**. Every note block cites the source section (for example, Textbook §1.1, Fig. 1.4, Table 1.2). Do not paste these notes into university submissions without your own wording.

## Local run

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

Open http://127.0.0.1:5000

## Deploy on Render

1. Push this folder to GitHub (see below).
2. On [Render](https://render.com) → **New Web Service** → connect the repository.
3. Settings:
   - **Runtime:** Python 3
   - **Build command:** `pip install -r requirements.txt`
   - **Start command:** `gunicorn app:app --bind 0.0.0.0:$PORT`
4. Deploy. Render sets `PORT` automatically.

You may also use `render.yaml` (Blueprint) from the dashboard.

## Push to GitHub

```bash
cd vtuhub-1baia103
git init
git add .
git commit -m "VTUHub 1BAIA103 Module 1 self-learning app"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo>.git
git push -u origin main
```

## Author

**Dr. Lokesh M R**, Professor, Department of Information Science & Engineering, A J Institute of Engineering and Technology, Mangaluru (VTU, Belagavi).

Class text: *Introduction to Artificial Intelligence and its Applications* (1BAIA103), Module 1 Part A.

Contact: lokeshmrmysore@gmail.com · [ORCID](https://orcid.org/0000-0003-0025-7941) · [GitHub](https://github.com/lokeshmr23)

## Course mapping

| Code | Title |
|------|--------|
| 1BAIA103 | Introduction to Artificial Intelligence and its Applications |
| Module 1 | What is AI, history, types of AI, ML vs programming, intelligence, applications |

Textbook used: *Module 1 Part A* (scanned class textbook supplied by the faculty).
