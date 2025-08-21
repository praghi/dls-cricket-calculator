# 🏏 DLS Cricket Calculator

A modern **Duckworth–Lewis–Stern (DLS) calculator** for limited-overs cricket matches (ODIs & T20s).  
Built with **FastAPI (backend)** and **Streamlit (frontend)**.

# 📜 Background – Duckworth–Lewis–Stern (DLS) Method
The Duckworth–Lewis method (D/L) was introduced in 1997 by two English statisticians, Frank Duckworth and Tony Lewis, to address fairness in rain-affected limited-overs cricket matches.Before D/L, cricket used methods like the Average Run Rate and Most Productive Overs (MPO), but both were flawed and often produced unfair results.The D/L method was formally adopted by the International Cricket Council (ICC) in 1999, making its debut in the 1999 Cricket World Cup.In 2014, the model was updated to Duckworth–Lewis–Stern (DLS), when Professor Steven Stern became the custodian and refined the system to better fit modern high-scoring cricket.Today, DLS remains the official ICC method for resetting targets in rain-interrupted One Day Internationals (ODIs) and T20 matches. 

# 🎯 Objective

This project aims to provide a free, easy-to-use DLS (Duckworth–Lewis–Stern) calculator for cricket enthusiasts, clubs, and local matches.

The motivation behind this project comes from a passion for both programming and cricket. During matches, it’s often confusing to understand how the revised targets are calculated when interruptions like rain occur.

By combining technical skills with a love for the game, this project offers a practical tool that anyone can use to quickly and accurately determine resources, par scores, and revised targets in real-time.

## 🚀 Features
- Supports **ODI (50 overs)** and **T20 (20 overs)**.
- Lookup **DLS resource percentage** by overs left & wickets lost.
- Calculate **Team 2 revised target** after rain interruptions.
- Extensible: JSON/CSV-based ICC resource tables.
- Ready for deployment (Streamlit Cloud, Docker, etc).


## 📂 Project Structure  

dls-cricker-calculator/
│── backend/ # FastAPI app  
│── frontend/ # Streamlit app  
│── data/ # Resource tables   
│── tests/ # Unit tests    
│── docker/ # Dockerfile + docker-compose
│── README.md  
│── requirements.txt  


## 🛠️ Installation

Clone repo:
```bash
git clone https://github.com/praghi/dls-cricket-calculator.git
``` 

Create virtual environment (using uv): 
```bash
uv venv
source .venv/bin/activate   # Mac/Linux
.venv\Scripts\activate      # Windows
```

Install dependencies: 
```bash
uv pip install -r requirements.txt
```   

FastAPI Backend (future)
```bash
uvicorn backend.main:app --reload
```   

▶️ Running the Apps  
```bash
streamlit run frontend/app.py
```

















