# api-telemetry-feature-store
This project represents an end-to-end Python system that simulates API telemetry traffic, ingests logs into Parquet format, and builds a Feature Store for real-time monitoring and anomaly detection.

## 📁 Project Structure
```
api-telemetry-feature-store/
│
├── .venv/                  <-- Virtual environment
├── data/                   <-- Raw log storage & Parquet files
│
├── src/                    <-- Core Python source modules
│   ├── __init__.py         <-- Package initializer
│   ├── generator.py        <-- Step 1: Telemetry log generator
│   ├── ingestion.py        <-- Step 2: Columnar storage ingestion (Parquet)
│   ├── features.py         <-- Step 3: Feature Store & SQL aggregates (DuckDB)
│   └── anomaly.py          <-- Step 4: ML Anomaly Detection (Isolation Forest)
│
├── app.py                  <-- Step 5: Streamlit monitoring dashboard
├── .gitignore              <-- Git ignore rules
├── README.md               <-- Project documentation
└── requirements.txt        <-- Python dependencies
```s
