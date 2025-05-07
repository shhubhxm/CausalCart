# CausalCart: Causal Inference & Pricing Strategy in Multi-Sided Marketplaces

**CausalCart** is a data science project that simulates a multi-sided marketplace and applies causal inference, uplift modeling, and pricing optimization to evaluate the impact of pricing, incentives, and ad placements on customer behavior and revenue. Built to reflect real-world experimentation frameworks like those used in companies such as Instacart, Uber, and Amazon.

---

## 🔍 Project Goals

- Simulate observational and experimental data in a multi-sided marketplace (customers, vendors, and advertisers)
- Apply causal inference techniques to measure treatment effects of pricing, discounting, and ad exposure
- Estimate customer LTV and retention using uplift modeling
- Use ML pipelines for classification, regression, and effect estimation
- Deploy interactive dashboards and automated A/B testing analysis

---

## ⚙️ Features

### 📈 Causal & Uplift Modeling
- Propensity score matching (PSM)
- Double ML with EconML / CausalML
- Uplift modeling using `XGBoost`, `sklearn`, and `TensorFlow`
- Heterogeneous treatment effect estimation

### 💡 Business Impact Modeling
- Elasticity estimation & price sensitivity analysis
- Product substitution modeling using regression trees
- Customer churn and retention modeling

### 📊 Data Simulation & A/B Testing
- Simulated observational + randomized experiment datasets
- Controlled experiments with random assignment + post-treatment adjustments
- Synthetic multi-sided marketplace simulation: buyers, sellers, ads

### 🧪 Experimentation Dashboard
- Streamlit dashboard to compare treatment/control outcomes
- Average Treatment Effect (ATE), Conditional ATE, uplift scores
- A/B test monitoring with metrics like revenue, retention, and conversion

---

## 🧰 Tech Stack

| Layer               | Tools & Frameworks                                 |
|--------------------|----------------------------------------------------|
| ML & Causal Tools  | EconML, CausalML, Scikit-learn, XGBoost, TensorFlow|
| Data Pipelines      | Pandas, SQL, NumPy                                 |
| Experimentation     | A/B test simulation, DoubleML, PSM                 |
| Dashboard & Viz     | Streamlit, Matplotlib, Plotly                      |
| Deployment          | Docker, GitHub Actions (CI/CD optional)           |

---

## 📁 Project Structure

```

CausalCart/
├── data/
├── notebooks/
├── src/
│   ├── pipelines/
│   ├── models/
│   ├── experiments/
│   └── dashboards/
├── streamlit\_app/
├── tests/
├── requirements.txt
└── README.md

````

---

## 🧪 Key Use Cases

- Evaluate impact of discounts or ads on user retention
- Measure effect of price changes on conversion (price elasticity)
- Determine whether high spenders respond differently to promotions
- Simulate policy interventions for multi-party outcomes

---

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/yourusername/CausalCart.git
cd CausalCart

# Install dependencies
pip install -r requirements.txt

# Launch dashboard
streamlit run streamlit_app/main.py

