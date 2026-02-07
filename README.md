# Big Data Architecture + Retail Value-in-Analytics Blueprint

## Overview
This repository contains a two-part blueprint:
1) A big-data platform recommendation for an e-commerce company (Veloxa&Co) needing real-time analytics with limited in-house programming expertise.
2) A retail value-in-analytics plan for a physical store (PriMarket) using Wi-Fi, RFID, and third-party POI signals to drive operational improvements and customer value.

## Part A — Veloxa&Co: Big Data Platform Recommendation

### Problem
Veloxa&Co generates large volumes of sales and behavioural data and needs real-time insights for pricing and promotions. The solution must be scalable, cost-conscious, and usable by teams with limited programming skills.

### Options Compared
- Hadoop (HDFS + MapReduce): strong for batch jobs but slower for real-time needs and heavier on coding/ops.
- Spark: in-memory processing with streaming support for real-time + batch analytics.
- Cloud platforms: managed services with elastic scaling and pay-as-you-go cost structure.

### Recommendation
- Use a cloud-managed Apache Spark environment for performance and scalability.
- Prioritise SQL-first access via Spark SQL / Hive for usability.
- Enable optional web-based ad-hoc analytics through cloud SQL services (e.g., Athena/BigQuery) for non-technical teams.

### Value
This design improves speed-to-insight, reduces operational overhead, and lowers adoption friction by using familiar SQL patterns.

## Part B — PriMarket: Value Creation using Wi-Fi, RFID and POI Data

### Wi-Fi Analytics (In-store Movement)
- Uses zone-based access point data to reconstruct traffic flow, dwell times and congestion.
- Business value: heatmaps, layout optimisation, identifying underperforming areas, and improving conversion by fixing friction points.
- Customer value: smoother navigation and real-time personalised offers when linked to a loyalty app.

### RFID Analytics (Merchandise Flow)
- Tracks item movement across key store checkpoints (backroom, replenishment, cashier, exit).
- Business value: real-time inventory accuracy, replenishment optimisation, product lifecycle insights, and loss prevention.
- Customer value: higher availability confidence and faster checkout via multi-item scanning.

### Third-party POI Signals
- Uses external check-in patterns to infer lifestyle segments, competitor overlap, partnership opportunities and expansion signals.
- Supports more context-aware personalisation and strategic planning beyond in-store behaviour alone.

## What this demonstrates
Data strategy and system thinking: selecting fit-for-purpose platforms, designing SQL-accessible analytics, and translating behavioural + operational signals into measurable business and customer value.
