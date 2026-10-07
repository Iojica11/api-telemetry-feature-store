# api-telemetry-feature-store
This project represents an end-to-end Python system that simulates API telemetry traffic, ingests logs into Parquet format, and builds a Feature Store for real-time monitoring and anomaly detection.

## 📁 Project Structure
```
api-telemetry-feature-store/
│
├── .venv/                  
├── data/                   <-- Raw log storage & Parquet files
│
├── src/                    <-- Core Python source modules
│   ├── __init__.py         <-- Package initializer
│   ├── generator.py        <-- Telemetry log generator
│   ├── ingestion.py        <-- Columnar storage ingestion (Parquet)
│   ├── features.py         <-- Feature Store & SQL aggregates (DuckDB)
│   └── anomaly.py          <-- ML Anomaly Detection (Isolation Forest)
│
├── app.py                  <-- Streamlit monitoring dashboard
├── .gitignore              <-- Git ignore rules
├── README.md               <-- Project documentation
└── requirements.txt        <-- Python dependencies
```
