# 🏦 SME Investment Intelligence Platform

> A full-stack data analytics and AI platform for tracking SME investments, risk, and development impact across East Africa.

🌐 **[View Live Dashboard](https://mochwada.github.io/sme-investment-platform/dashboard/sme_dashboard.html)**

---

## 📌 Overview

The **SME Investment Intelligence Platform** is a production-grade analytics system built to support investors, fund managers, M&E specialists, and development finance institutions with real-time intelligence on SME portfolio performance, risk exposure, and development impact across East Africa.

Built on **Supabase PostgreSQL**, **IBM Watsonx**, and **Python**, the platform tracks 500 SMEs across 6 countries with over 20,000 records of investments, repayments, performance snapshots, impact metrics, and AI-generated risk scores.

---

## 🚀 Live Dashboard

The interactive dashboard features **7 tabs** powered by live data:

| Tab | What it shows |
|-----|--------------|
| **Overview** | Portfolio KPIs, revenue trends, gender inclusion, capital by type |
| **Sector Intelligence** | Capital, revenue, profit margin, default rate by sector |
| **Risk Intelligence** | Risk bands, loan aging (PAR), exposure concentration, repayment |
| **M&E Impact** | Jobs, women & youth employment, SDG alignment, cost per beneficiary |
| **Portfolio** | Investor scorecard, default rates, full portfolio breakdown |
| **SME Directory** | Top 50 SMEs ranked by repayment score with full scorecard |
| **🗺 Geography** | Interactive Leaflet map — 500 SMEs across East Africa |

---

## 🗄️ Database Schema (Supabase PostgreSQL)

| Table | Records | Description |
|-------|---------|-------------|
| `sme_sectors` | 25 | Agriculture, Trade, Manufacturing, Services, Tech |
| `sme_regions` | 30 | Cities across Kenya, Uganda, Tanzania, Rwanda, Ethiopia, S.Sudan |
| `sme_investors` | 15 | DFIs, Microfinance, VCs, Banks, NGOs |
| `smes` | 500 | Full SME profiles with correct sector mapping |
| `sme_investments` | 1,200 | Loans, grants, equity disbursements |
| `sme_repayments` | 11,520 | Monthly payment records with late flags |
| `sme_performance` | 4,000 | Quarterly revenue, expenses, employee snapshots |
| `sme_impact` | 2,000 | Annual jobs, women/youth employment, SDG alignment |
| `sme_risk_scores` | 1,200 | AI default probability + risk bands |

---

## 🤖 Machine Learning Models

Trained in **IBM Watsonx / Google Colab** (Python + scikit-learn):

| Model | Algorithm | Purpose |
|-------|-----------|---------|
| Default Risk Predictor | Random Forest Classifier | Predict probability of loan default |
| Growth Score | Feature Engineering | SME expansion potential |
| Impact Score | Composite index | Development impact measurement |

**Model accuracy:** 77.9% on high-risk SMEs, 4.8% false positive on stable SMEs.

---

## 🧰 Tech Stack

| Layer | Technology |
|-------|-----------|
| **Database** | Supabase PostgreSQL (9 tables, 20,500+ records) |
| **API** | Supabase Edge Functions (Deno/TypeScript) — 18 queries |
| **ML / AI** | IBM Watsonx + Google Colab (Python, scikit-learn) |
| **Dashboard** | Vanilla HTML, CSS, JavaScript + Chart.js + Leaflet.js |
| **Hosting** | GitHub Pages (free, no server) |

---

## 📊 Key Numbers

```
💰 Total Capital Deployed    : KES 1,299,874,000
📊 Total Investments         : 1,200
🏢 SMEs Tracked              : 500
🌍 Countries Covered         : 6
⚠️  Default Rate              : 10.0%
👷 Total Jobs Created         : 4,992
👩 Women Employed             : 2,916
🎓 Youth Employed             : 2,606
🗺️  Cities on Map             : 30
```

---

## 📁 Repository Structure

```
sme-investment-platform/
├── README.md
├── .gitignore
├── dashboard/
│   └── sme_dashboard.html
├── notebooks/
│   ├── 01_sme_data_exploration.ipynb
│   ├── 02_sme_portfolio_analysis.ipynb
│   └── 03_sme_impact_report.ipynb
└── docs/
    └── enhancement_plan.pdf
```

---

## 🖥️ Getting Started

```bash
git clone https://github.com/Mochwada/sme-investment-platform.git
```

Open `dashboard/sme_dashboard.html` in any browser — no server or installation needed.

---

## 👤 Author

Built by **Mark Ochwada**
- 💼 LinkedIn: [linkedin.com/in/mark-ochwada](https://www.linkedin.com/in/mark-ochwada-b3a1b3198/)
- 🐙 GitHub: [github.com/Mochwada](https://github.com/Mochwada)

---

## 📄 License

MIT License — free to use, modify, and share with attribution.
