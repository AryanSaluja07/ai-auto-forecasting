# 🚗 AI-Powered Vehicle Sales Forecasting & Inventory Optimization

## 1. Business Problem
The dealership network struggles with mismatched inventory:
- Some car models are overstocked and tie up capital in storage.
- Other models frequently go out of stock, causing missed sales and dissatisfied customers.
- Decision-making is largely manual and based on historical intuition, not real-time data.

The company wants to **use Artificial Intelligence (AI)** to forecast vehicle demand and support **data-driven inventory decisions**.

---

## 2. Business Objectives
1. Forecast monthly demand per **model × branch** with high accuracy.  
2. Identify factors influencing demand (season, fuel type, price, etc.).  
3. Recommend an **inventory optimization policy** (stocking levels, transfers).  
4. Provide a **dashboard** for executives to visualize trends.  
5. Build an **AI chatbot concept** that allows dealership managers to query forecasts conversationally.

---

## 3. Scope
### In-Scope
- New vehicle sales data (no used-car or service data).  
- Forecasting horizon: next 3 months.  
- Branches: all existing dealership locations in dataset.  
- Integration with AI/ML models (Prophet, XGBoost).  
- Power BI/Tableau dashboard.  
- Chatbot concept prototype (Streamlit or mockup).

### Out-of-Scope
- Real-time integration with ERP systems.  
- Price optimization or marketing campaign prediction.  
- Fleet/rental sales.

---

## 4. Stakeholders
| Role | Interest / Responsibility |
|------|---------------------------|
| **Head of Sales** | Oversees performance, approves inventory targets |
| **Branch Managers** | Manage stock & sales at local level |
| **Inventory Planner / Supply Chain Team** | Uses forecasts to reorder or transfer vehicles |
| **Finance Team** | Monitors carrying costs |
| **Data & IT Team** | Supports data integration and dashboard infrastructure |

---

## 5. Key Business Questions
1. What models are predicted to sell most in each region next month?  
2. Which branches will face overstock or stockout situations?  
3. How do seasonal and fuel-type trends affect sales?  
4. How can AI forecasts reduce manual planning effort?  
5. What process improvements can be automated through a chatbot interface?

---

## 6. Success Criteria / KPIs
| KPI | Target | Description |
|------|---------|-------------|
| **MAPE (Mean Absolute Percentage Error)** | ≤ 10 % | Forecast accuracy measure |
| **Overstock Reduction** | ≥ 20 % improvement | Compared to baseline inventory cost |
| **Stockout Reduction** | ≥ 15 % improvement | Missed-sale reduction |
| **Dashboard Adoption Rate** | ≥ 90 % | Branch managers using dashboard weekly |
| **Chatbot Response Accuracy** | ≥ 80 % correct intents | For pilot demo |

---

## 7. Constraints & Assumptions
- Historical sales data is complete and reliable.  
- External factors (fuel prices, marketing) may change but not drastically.  
- Forecasts will be refreshed monthly.  
- Chatbot responses rely on static forecast data (not live retraining).  

---

## 8. Deliverables
| Deliverable | Description |
|--------------|-------------|
| **Clean dataset** | `data/car_sales_clean.csv` |
| **Forecast results** | `data/prophet_forecasts.csv` |
| **Power BI/Tableau Dashboard** | Interactive visualization |
| **Chatbot Prototype** | Streamlit demo for natural-language queries |
| **Reports & Docs** | BRD, Insights Report, Process Diagrams, Presentation |

---

## 9. Timeline (3 Weeks)
| Week | Focus | Key Output |
|------|--------|-------------|
| **1** | Data Prep & EDA | Clean dataset, EDA visuals |
| **2** | AI Modeling & Dashboard | Forecast outputs, Power BI dash |
| **3** | Insights & Chatbot | Recommendations, Chatbot demo, Presentation |

---

## 10. Risks & Mitigation
| Risk | Mitigation |
|-------|-------------|
| Data quality issues | Data validation & outlier handling |
| Model underperformance | Use ensemble approach (XGBoost + Prophet) |
| Stakeholder adoption barriers | Deliver simple dashboards & training |
| Tech limitations | Prototype locally with sample data before scaling |

---

## 11. Expected Benefits
- Reduced inventory carrying costs.  
- Improved cash flow and sales turnover.  
- Faster decision cycles using AI forecasts and chatbot queries.  
- Stronger data-driven culture within dealership network.
