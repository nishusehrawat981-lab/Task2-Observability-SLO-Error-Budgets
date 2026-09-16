# Task 2 — Observability Deep-Dive, SLOs & Error Budgets

## Overview

This project builds a semantic metric layer and data-quality monitoring framework.

The main objective is to make sure that different people asking the same business question receive the same metric definition and result.

## Task Objective

The project focuses on:

- Semantic metrics
- Metric definitions
- Data sources
- Refresh frequency
- Decision usage
- Data freshness
- Data volume
- Null values
- Uniqueness
- Quality alerts

## Dataset

The metric dictionary contains information about each metric.

Important fields include:

- metric
- definition
- source
- refresh
- decision_use

The data-quality test dataset contains:

- test
- field
- threshold
- observed
- status
- action

## Analysis Performed

### 1. Metric Dictionary

Each metric has:

- One definition
- A source
- A refresh expectation
- A business decision use

This creates a single source of truth for metrics.

### 2. Data Quality Monitoring

The following quality dimensions were checked:

- Freshness
- Volume
- Null rate
- Uniqueness

### 3. Quality Test Validation

Each quality test contains:

- Expected threshold
- Observed value
- PASS/FAIL status
- Required action

### 4. Quality Pass Rate

The overall quality pass rate is calculated as:

passed tests / total tests

## Important Metrics

### Freshness

Measures whether the latest available data is recent enough.

### Volume

Checks whether the expected amount of data has arrived.

### Null Rate

Checks for missing values in important fields.

### Uniqueness

Checks whether duplicate records exist where unique records are expected.

## Visualizations

The project includes a data-quality test result chart showing:

- Passed tests
- Failed tests

## Business Actions

The monitoring system should:

1. Alert when data becomes stale.
2. Detect unexpected changes in data volume.
3. Identify important null values.
4. Detect duplicate records.
5. Connect every alert to a specific action.

## Tools Used

- Python
- Pandas
- Matplotlib
- Google Colab

## Files

- Task2_Metric_Dictionary_Demo.csv
- Task2_Data_Quality_Tests_Demo.csv
- Task2_Observability_SLO_Error_Budget_Report_Demo.pdf
- Task2_Answer_to_Submit.txt

## Conclusion

A centralized metric layer and automated data-quality checks help create consistent and reliable analytics.

The objective is that two people asking the same question should receive the same number because the metric definition is standardized.
