# 🍽️ Petpooja AI Ecosystem

> AI-Powered Restaurant Management Platform with Analytics Dashboard & On-Device Voice POS

![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)
![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)
![WebGPU](https://img.shields.io/badge/WebGPU-Enabled-green)
![Streamlit](https://img.shields.io/badge/Streamlit-1.0+-FF4B4B?logo=streamlit)
[![Live Demo](https://img.shields.io/badge/🚀%20Live%20Demo-Module%201-FF4B4B?style=for-the-badge)](YOUR_STREAMLIT_URL_HERE)

---

## 🌐 Live Demo

| Module | Status | Link |
|--------|--------|------|
| 📊 **Module 1** — Owner Intelligence Dashboard | ✅ Deployed | [**👉 Open Live App**](YOUR_STREAMLIT_URL_HERE) |
| 🤖 **Module 2** — AI Revenue Copilot | 🖥️ Run Locally | See setup below |

> 💡 **Tip for Module 1:** Upload your own `menu_master.csv` and `sales_data.csv` to see the dashboard in action, or use the sample data preloaded by default.

---

## 📋 Overview

A dual-module AI platform built for restaurant owners and staff:

| Module | Purpose | Tech Stack |
|--------|---------|------------|
| **Module 1** | Owner Intelligence Dashboard | Python, Streamlit, Scikit-Learn, Plotly |
| **Module 2** | AI Revenue Copilot (Voice POS) | React 19, Vite, WebGPU, HuggingFace Transformers.js |

---

## 📊 Project Statistics

| Metric | Value |
|--------|-------|
| Total Lines of Code | **3,032** |
| Menu Items (SKUs) | **35** across **11 categories** |
| Transaction Records | **121** line items |
| Unique Customers | **30+** |
| Cuisines Covered | **6** (North Indian, Gujarati, Chinese, South Indian, Continental, Other) |
| LLM Model Size | **~350 MB** (quantized, cached locally) |
| Association Rules | **8** co-purchase rules (lift: 1.7x–3.1x) |

---

## 🚀 Module 1: Owner Intelligence Dashboard

A powerful analytics suite built in Python that ingests POS data to optimize menu pricing, identify customer segments, and forecast future demand.

### Features
| Feature | Description |
|---------|-------------|
| 📊 **BCG Menu Engineering** | Classify items into Stars, Plowhorses, Puzzles & Dogs |
| 👥 **RFM Customer Segmentation** | Champions, Loyal, At Risk, Lost segments |
| 📈 **ML Demand Forecasting** | Linear Regression price-demand predictions |
| 💰 **Price Simulator** | Real-time profit impact analysis |
| 🔥 **Smart Combo Generator** | Co-purchase frequency based recommendations |
| 🎯 **Upsell Engine** | Auto-generates `upsell_config.json` for POS integration |
| 📉 **Cohort Retention Heatmaps** | Track customer retention over time |
| 🏷️ **Discount Engine** | Optimal discount strategies by segment |

### 🌐 Live Demo
> **[👉 Click here to open the live dashboard](YOUR_STREAMLIT_URL_HERE)**

### Run Locally
```bash
cd "Module01-Owner_ Intelligence _Dashboard"
pip install -r requirements.txt
streamlit run app.py
```

---

## 🤖 Module 2: AI Revenue Copilot

A **100% offline**, WebGPU-powered Voice/Text Point-of-Sale (POS) interface for restaurant staff with on-device NLP.

### Features
| Feature | Description |
|---------|-------------|
| 🎤 **Voice Ordering** | Web Speech API for hands-free order capture |
| 🧠 **On-Device LLM** | SmolLM2-360M running 100% offline via WebGPU |
| 📊 **Revenue Dashboard** | KPI cards, profit charts, BCG scatter matrix |
| 🛒 **Smart Upsell Engine** | Real-time context-aware suggestions |
| 🎫 **KOT Manager** | Kitchen Order Ticket generation |
| 📋 **Menu Setup** | Full item-level margin analysis |

### AI Specifications
| Spec | Value |
|------|-------|
| Model | SmolLM2-360M-Instruct (HuggingFace) |
| Size | ~350 MB (quantized q4f16) |
| Inference | 100% browser-side via WebGPU |
| Execution | Dedicated Web Worker (non-blocking UI) |

### Run Module 2
```bash
cd "Module 2 Node.js + React"
npm install
npm run dev
```
Then **Ctrl + Click** on the localhost link (e.g., `http://localhost:5173`)

---

## ⚠️ Important Setup Notes

### For Module 2 (AI Revenue Copilot)
1. **Browser:** Use Google Chrome or Microsoft Edge with WebGPU support
2. **GPU Acceleration:** Ensure "Use graphics acceleration when available" is **ON** in browser settings
3. **First Run:** Navigate to "Voice Copilot" tab and type a test order — the browser will download the AI model (~350MB) and cache it
4. **Offline Test:** After initial load, **disconnect Wi-Fi** and place another order to verify 100% offline NLP

---

## 📁 Project Structure

```
Petpooja AI Ecosystem/
├── Module 1 Streamlit/
│   ├── app.py                    # Analytics dashboard (934 lines)
│   ├── petpooja_pos_data.csv     # POS transaction data
│   └── upsell_config.json        # Auto-generated upsell rules
│
├── Module 2 Node.js + React/
│   ├── src/
│   │   ├── petpooja-copilot.jsx  # Main React app (1,807 lines)
│   │   └── worker.js             # WebGPU LLM worker (67 lines)
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

---

## 🛠️ Tech Stack

| Module 1 | Module 2 |
|----------|----------|
| Python 3.9+ | React 19 + Vite 7 |
| Streamlit | HuggingFace Transformers.js |
| Pandas | WebGPU |
| Plotly | Web Speech API |
| Scikit-Learn | Recharts |
| NumPy | Lucide React |

---

## 🧮 Algorithms Implemented

| Algorithm | Module | Purpose |
|-----------|--------|---------|
| BCG Matrix Classification | 1 & 2 | Menu item categorization |
| Linear Regression | 1 | Demand forecasting |
| RFM Segmentation (Quartile) | 1 | Customer segmentation |
| Association Analysis (Lift) | 1 & 2 | Combo recommendations |
| Price Elasticity Simulation | 1 | Profit optimization |
| Cohort Analysis | 1 | Retention tracking |

---

## 👨‍💻 Author

Built for the **Petpooja AI Hackathon**

---

## 📄 License

MIT License