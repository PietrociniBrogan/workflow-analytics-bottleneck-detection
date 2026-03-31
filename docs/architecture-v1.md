# Architecture Note v1

## Goal

Create a workflow analytics platform that transforms raw workflow event data into usable metrics for bottleneck detection and process monitoring.

## Source Data

Initial source data will be synthetic and stored as CSV and/or JSON files.

## Flow

1. Raw source files are stored in `data/raw`
2. Python ingestion script reads files
3. Validation checks required fields, types, missing values, and bad records
4. Cleaned data moves into staging outputs
5. SQL models transform staging data into core analytical tables
6. Metrics are calculated from core tables

## Planned Layers

- raw
- staging
- core
- marts

## Initial Technical Stack

- Git/GitHub
- Python
- SQL
- Later: Postman, JS/TS, dbt-style layout, Snowflake, Databricks

## Risks / Assumptions

- event ordering must be consistent
- stage transitions need clear definitions
- synthetic data must be realistic enough to support meaningful metrics
