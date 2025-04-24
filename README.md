# ✏️ Handwritten Math Expression Solver

This is a full-stack application that lets users **draw mathematical expressions** on a canvas, processes the drawings using **Generative AI**, and returns the **calculated results** dynamically. The frontend is built with **React + Mantine** and the backend with **FastAPI**, leveraging **Google's Generative AI** for interpreting handwritten input.

---

## 🧠 Features

- 🎨 Draw math expressions directly on a canvas (supports color and erasing)
- 🤖 Uses Google Generative AI to recognize handwritten expressions
- 🔢 Calculates both evaluated expressions and variable assignments
- 🧮 Displays results using LaTeX rendered via MathJax
- 📦 Clean integration between frontend and backend using Axios

---

## 🧰 Tech Stack

**Frontend**
- React (TypeScript)
- Mantine UI
- MathJax for LaTeX rendering
- Axios for API calls
- Draggable for moving rendered LaTeX
- Tailwind CSS for styling

**Backend**
- FastAPI
- Python 3.11+
- Google Generative AI API (Gemini)
- Pillow (image preprocessing)

---

## 🚀 Getting Started

### 📦 Backend Setup (`calc-be-main`)

```bash
# 1. Navigate to the backend folder
cd calc-be-main

# 2. Create virtual environment
python -m venv env
source env/bin/activate  # Windows: env\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Set environment variable
export GOOGLE_API_KEY=your_api_key_here  # Or use a .env file

# 5. Run FastAPI server
uvicorn main:app --reload
