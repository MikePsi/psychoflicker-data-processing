psychoflicker-data-pipeline is a modular workflow for taking raw Psychoflicker experimental logs all the way through to subject-level summary metrics and visualizations. It consists of three key stages:

Data Ingestion & Cleaning

Load raw CSV/JSON exports of trial events for each session

Standardize variable names, timestamps, and trial codes

Handle missing data and flag outlier responses

Dataset Assembly & Manipulation

Merge pre- and post-session files by subject and condition

Compute trial-wise deltas (e.g. reaction time changes)

Aggregate into a single “long” format DataFrame for analysis

Analysis & Reporting

Calculate per-subject trial counts, means, and variances

Generate summary tables and diagnostic plots

Export ready-to-share CSVs and figures for publication

Each notebook focuses on one stage of the pipeline, with clear dependency ordering and reusable utility functions; simply run them in sequence to reproduce the full analysis from raw data to final summaries.
