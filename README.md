## Overview
This project performs a reproducible analysis of student learning trajectories using the Open University Learning Analytics Dataset (OULAD). It aggregates virtual learning environment (VLE) logs into daily engagement trajectories, visualizes cohort-level patterns, and explores early-warning signals using descriptive statistics and clustering.

## Data
This project uses the OULAD dataset.
Required files:
- studentInfo.csv
- studentVle.csv

Data files should be placed under:
data/raw/

Due to data usage restrictions, raw data files are not included in this repository.

## Methods
- Filtered to a single course presentation (AAA 2013J)
- Aggregated VLE click events into per-student daily engagement counts
- Applied rolling mean smoothing to reduce day-to-day noise
- Normalized trajectories at the student level
- Visualized cohort-level engagement using:
  - Mean ± standard deviation bands
  - Median and interquartile range bands
- Explored trajectory pattern grouping using KMeans clustering

## Outputs
The analysis produces figures that summarize cohort-level engagement trends and trajectory patterns, suitable for use in research briefs or presentations.

## Reproducibility
All analysis code is designed to be reproducible using Python and Jupyter notebooks. Figures can be regenerated from raw data following the documented workflow.
