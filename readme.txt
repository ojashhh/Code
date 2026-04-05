Now I have everything I need. Let me build a comprehensive Streamlit app with a polished frontend.Here's your complete Streamlit app. Run it with:

```bash
streamlit run credit_risk_app.py
```

---

**What's inside — 4 tabs:**

**📊 Overview & EDA** — Dataset KPI cards, default distribution bar chart, interest rate histogram by class, income vs loan scatter, correlation heatmap, credit score KDE curves. All styled dark with a gold/orange palette.

**🤖 Model Training** — One click trains all 4 models (Logistic Regression, Random Forest, XGBoost, XGBoost Balanced). Results appear in a styled leaderboard table with green highlights on best Recall/ROC-AUC/F1. Download buttons export the `.joblib` model and scaler directly.

**📈 Results & Insights** — ROC curves for all 4 models overlaid, threshold-adjusted confusion matrix, top-12 feature importance bar chart, and a live **Precision/Recall/F1 vs Threshold** sensitivity curve — all react to the sidebar threshold slider.

**🎯 Live Prediction** — Fill in 16 applicant fields across 3 columns, hit "Assess Risk", and get: default probability, a colored HIGH/LOW RISK badge, a gradient gauge bar, and flagged risk signals (high LTI, low credit score, high DTI, etc.).

The sidebar controls test split % and decision threshold globally across all tabs.















No, you just need **Python** (3.8+) installed. Everything else is pure Python packages installed via pip.

Run this once to install all dependencies:

```bash
pip install streamlit xgboost scikit-learn pandas numpy matplotlib seaborn joblib
```

Then launch the app:

```bash
streamlit run credit_risk_app.py
```

Streamlit will automatically open your browser. That's it — no external tools, databases, or system dependencies needed.

One small note: the app is hardcoded to look for your dataset at the path `/mnt/user-data/uploads/...` (a container path). When running locally, just use the **"Upload loan CSV"** file uploader in the sidebar instead — it works the same way.