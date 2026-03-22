# Strategic Explainable Electricity Load Forecasting ⚡

## Overview
Energy load forecasting models are typically evaluated using predictive accuracy metrics such as RMSE and MAE. However, high forecasting performance does not necessarily imply alignment with long-term sustainability objectives.

This project introduces the **Strategic Alignment Score (SAS)** — a novel metric that evaluates how well machine learning models align with sustainability-driven energy planning goals.

Using explainable AI techniques (SHAP and LIME), we analyze how different models make predictions and assess their strategic relevance.

---

## 🎯 Objectives

- Build accurate electricity load forecasting models
- Apply explainable AI (SHAP & LIME)
- Map model features to **policy-relevant strategic categories**
- Develop a new evaluation metric (**SAS**)
- Compare models on both **accuracy and strategic alignment**

---

## 📊 Models Used

- XGBoost
- Reduced XGBoost
- Random Forest
- LSTM (Deep Learning)

---

## 🧠 Key Concept: Strategic Alignment Score (SAS)

Features are grouped into three strategic categories:

- **Reactive** → Short-term demand (Lag features)
- **Climate** → Temperature, humidity (cooling demand)
- **Structural** → Time-based patterns (hour, day)

SAS measures how much a model relies on these groups, enabling evaluation beyond accuracy.

---

## 📈 Results

| Model           | RMSE | SAS  |
|----------------|------|------|
| XGBoost        | ~29  | 0.21 |
| Reduced XGB    | ~33  | 0.22 |
| Random Forest  | ~30  | 0.20 |
| LSTM           | ~51  | 0.33 |

### Key Findings

- Tree-based models → High accuracy, low strategic alignment  
- LSTM → Lower accuracy, higher strategic alignment  
- Clear **accuracy vs interpretability trade-off**

---

## 🔍 Explainability

- **SHAP** → Global feature importance
- **LIME** → Local prediction explanations
- Feature contributions mapped to **Strategic KPIs**

---

## 📊 Additional Analysis

- Statistical testing (bootstrap confidence intervals)
- Entropy analysis of explanations
- Scenario-based SAS weighting
- Multi-model comparison

---

## 💡 Key Insights

- High accuracy ≠ strategic usefulness
- Model architecture influences reasoning behavior
- SAS provides a bridge between ML models and real-world policy decisions
- LSTM models better capture long-term planning signals

---

## 🧪 Research Questions

- Can SHAP feature importance be mapped into strategic categories?
- Do different models produce different strategic alignment levels?
- Does SAS improve interpretability over raw SHAP?

---

## 🧾 Contributions

1. Proposed **Strategic Alignment Score (SAS)**
2. Demonstrated accuracy–alignment trade-off
3. Integrated explainable AI with energy policy evaluation
4. Compared tree-based vs deep learning models for strategic reasoning

---

## ⚙️ Installation

```bash
pip install -r requirements.txt
