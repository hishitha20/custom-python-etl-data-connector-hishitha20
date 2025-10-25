# RIPEstat ETL Connector

**Author:** K Hishitha  
**Roll No:** 12345  Section: A

## What this does
- Extracts AS overview data from the RIPEstat public API
- Transforms and stores the raw JSON into a MongoDB collection `ripestat_raw`
- Adds `ingested_at` timestamp for auditability

## Files
- `etl_connector.py` - main ETL script
- `ENV_TEMPLATE` - sample env keys (no secrets)
- `.env` - local secret file (do not commit)
- `requirements.txt` - Python dependencies

## How to run
1. Create and activate venv:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
