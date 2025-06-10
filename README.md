# Advanced Simulation Assignments

This project comprises Python code from three consecutive assignments completed in the course **Advanced Simulation** of the MSc programme *Engineering and Policy Analysis* at TU Delft. The model analyses Bangladesh's road network using Road Maintenance Management System (RMMS) data to compute vulnerability and criticality metrics.

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

The `data` directory referenced in the scripts is not included because the datasets are large.

## Methods Overview
The workflow is divided over the three assignments:
1. **Data collection and cleaning** – Scripts such as `data_pull.py`, `data_clean.py` and `bridge_condition_refactored.py` parse the RMMS `.htm` files and generate processed CSV datasets.
2. **Vulnerability and criticality computation** – `merging_vulnerability_roads.py` combines hazard scores with road attributes, and `Compute_metrics.py` calculates normalized indicators for roads and bridges.
3. **Reporting** – Rankings of the most critical and vulnerable links are saved to the `analysis` folder and summarised in the report under `Report/`.

## Usage
Install the required packages with:
```bash
pip install -r requirements.txt
```
Then run the scripts in `model/` following the order described above. Adjust the paths to the RMMS data files locally.

## Modifying Inputs
You can adjust hazard weights or road condition categories by editing the data and scripts inside `model/`.

## Notes on Data
The raw and processed datasets are not included in this repository because of their size.

## Acknowledgments
This project is based on the **EPA133a - Advanced Simulation** course at TU Delft.
