# HireCue — BI & AI Analytics Dashboard

An interactive **Business Intelligence and AI analytics platform** developed for **HireCue**, a recruitment management platform.

The project provides a centralized analytical view of recruitment activities, candidate pipelines, AI usage, system events, platform operations, and workforce forecasting.

## About the Project

The dashboard transforms operational HireCue data into interactive visualizations and analytical insights.

It combines **Power BI**, **MySQL**, and an **AI Workforce Forecasting service** to monitor recruitment performance, platform activity, AI consumption, and key business indicators.

The AI forecasting component uses historical daily metrics to predict important HireCue KPIs and supports the analysis of future platform activity.

## Main Features

### Recruitment Analytics

- Recruitment pipeline monitoring
- Candidate application analysis
- Average candidate score comparison
- Job offers by status
- Job offers by position type
- Candidate pipeline analysis

### Platform & System Monitoring

- Overview of system events
- Recent activity logs
- Platform activity monitoring
- AI-generated task monitoring
- Recruitment operations tracking

### AI Performance Analytics

- LLM call monitoring
- AI token consumption
- AI cost analysis
- AI provider comparison
- AI usage monitoring

### AI Workforce Forecasting

- Daily workforce KPI aggregation
- Historical KPI analysis
- Future KPI forecasting
- LSTM and GRU model comparison
- MAE, RMSE and MAPE evaluation
- Automatic selection of the best-performing model

### Workforce KPIs

The forecasting service analyzes and predicts:

- Jobs created
- Total applications
- AI tokens
- AI cost
- LLM calls
- Revenue proxy
- Active subscriptions
- Completed events
- Active recruiters
- Active companies

## Technology Stack

### Business Intelligence

- Power BI
- Power BI Service
- Data Visualization
- DAX
- Interactive Dashboards

### Database

- MySQL
- SQL
- Relational Data Modeling

### AI & Machine Learning

- Python
- TensorFlow
- Keras
- LSTM
- GRU
- Scikit-learn
- Pandas
- NumPy

### Backend & API

- FastAPI
- Node.js
- Express.js
- REST APIs
- JWT Authentication

### Frontend

- React.js

## Data Architecture

```text
                 ┌──────────────────────┐
                 │     HireCue OLTP     │
                 │       MySQL          │
                 └──────────┬───────────┘
                            │
              ┌─────────────┴─────────────┐
              │                           │
              ▼                           ▼
     ┌──────────────────┐       ┌────────────────────┐
     │     Power BI     │       │ AI Forecasting     │
     │    Analytics     │       │      Service       │
     └────────┬─────────┘       └─────────┬──────────┘
              │                           │
              │                           ▼
              │                  ┌────────────────────┐
              │                  │ Daily Workforce    │
              │                  │ Metrics             │
              │                  └─────────┬──────────┘
              │                            │
              │                    ┌───────┴────────┐
              │                    │                │
              │                    ▼                ▼
              │                  LSTM              GRU
              │                    │                │
              │                    └───────┬────────┘
              │                            ▼
              │                  Model Comparison
              │                            │
              │                            ▼
              │                    Forecast Results
              │
              ▼
     ┌────────────────────────────────────────┐
     │      Recruitment & Business Insights   │
     └────────────────────────────────────────┘
```



---

## Demo




https://github.com/user-attachments/assets/43773340-31f1-40c9-b754-b9734cfeb11d




```
