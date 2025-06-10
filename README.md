# Advanced Simulation Assignments

This repository contains Python code and results for analysing the road network of Bangladesh. The model derives vulnerability and criticality scores for roads and bridges from the Road Maintenance Management System (RMMS) data. It was developed over three sequential assignments in the course **Advanced Simulation** of the MSc programme *Engineering and Policy Analysis* at TU Delft.

## Authors
- Alessandro Dell-Orto
- other author
- other author
- other author
- other author

## Repository Structure
- `model` – Python scripts for data processing and calculation of network metrics.
- `analysis` – CSV files with ranked criticality and vulnerability scores.
- `Images` – Plots created by the scripts.
- `Report` – Final report of the third assignment.
- `requirements.txt` – Python dependencies.

The `data` directory referenced in the scripts is omitted because the source datasets are large.

## Methods Overview
The analysis focuses on the road network of Bangladesh. The workflow is divided over the three assignments:
1. **Data collection and cleaning** – Scripts such as `data_pull.py`, `data_clean.py` and `bridge_condition_refactored.py` parse the RMMS `.htm` files, clean traffic and road condition tables, and create processed CSV datasets.
2. **Vulnerability and criticality computation** – `merging_vulnerability_roads.py` merges hazard scores for floods, river erosion and earthquakes with the processed road information. `Compute_metrics.py` calculates normalized criticality and vulnerability indicators for roads and bridges based on traffic, length and infrastructure condition.
3. **Reporting** – The resulting rankings of the most critical and vulnerable links are saved to the `analysis` folder and summarised in the report under `Report/`.

## Usage
Install the required packages with:
```bash
pip install -r requirements.txt
```
Then run the scripts in `model/` following the order described above to generate the processed datasets and metrics. Adjust the paths to the large RMMS data files locally before running the scripts.

## Notes on Data
The raw and processed datasets are not included in this repository because of their size. Place the required RMMS files under a `data` directory when executing the scripts.
