# 🧠 AI-Powered Logistics Pricing Engine

Built a dynamic pricing engine for SnappFood’s urban delivery network using ML-based zone clustering — optimized customer fees, biker compensation, and SLA targets across 300+ city regions.

---

## 📌 Overview

- **Company:** SnappFood (80K partners, 10M+ monthly orders)
- **Role:** Senior Product Manager – Led pricing engine design and rollout
- **Timeline:** 5-week build → 3-week pilot → scaled to 4 cities
- **Team:** 1 PM (me), 2 Data Scientists, 3 Backend Engineers, 1 BizOps Lead

---

## 🎯 Problem

Legacy pricing relied on:
- Manual zone configuration and static rates
- Misalignment between **customer delivery fees**, **partner payouts**, and **biker compensation**
- High SLA violation rates in certain zones

This led to underpaid couriers, overcharged customers, and poor delivery margins.

---

## 💡 Solution

Built a clustering-based pricing engine that:
- 📍 Segmented zones using both geographic data (area codes, traffic) and behavioral signals (SLA compliance, average ticket size)
- 🧠 Ran daily clustering jobs to group zones dynamically
- ⚖️ Balanced margins across stakeholders (customer, courier, partner)
- 🔄 Auto-updated rates via internal pricing API + dashboard

---

## 🛠️ Technologies Used

- **ML & Data Pipelines:** Python, Scikit-learn (clustering), Airflow, Pandas
- **Data Sources:** Order DB (PostgreSQL), Courier logs, SLA tracker
- **Infra:** Docker, GCP BigQuery, Firebase for config delivery
- **Monitoring:** Grafana dashboards, custom alerting via n8n

---

## 📈 Key Outcomes

| Metric                            | Result        |
|----------------------------------|---------------|
| Annual delivery cost savings     | ⬇️ 20%        |
| SLA violations                   | ⬇️ 35%        |
| Delivery fee fairness (Δ spread)| ⬇️ 48%        |
| Pricing simulation time          | ⬆️ 4× faster  |

Courier satisfaction increased in post-rollout surveys. Dynamic pricing also reduced churn in underperforming zones.

---

## 🔄 Long-Term Impact

- Adopted as default pricing logic for 70%+ of national zones
- Framework reused in warehouse routing + dispatch SLA tuning
- Used as baseline for Q1 2025 incentive budget modeling

---

## 📎 License

This case study is anonymized for portfolio demonstration. No raw geographic or financial data is disclosed.
