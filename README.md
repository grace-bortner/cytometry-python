Cytometry Analysis in Python

Flow and mass cytometry analysis pipeline in Python — from raw FCS files through quality control, dimensionality reduction, clustering, and differential abundance testing.

Status:
In active development. This repository is being built throughout 2026 as part of a computational immunology portfolio. Sections are added as the corresponding skills are developed across a 12-week Python + R learning plan. Target completion: August-September 2026.
Until then, this README serves as a planning document for the project's scope and structure. Code, notebooks, and figures will be added as each stage of the analysis is completed.

Project Goal:
To build a reproducible end-to-end cytometry analysis pipeline in Python, applied to a publicly available flow or mass cytometry dataset from FlowRepository, demonstrating the methodological steps used in high-dimensional immune profiling studies.

Planned Pipeline:
- Data loading — FCS file parsing with FlowKit or readfcs
- Quality control — bead removal, doublet exclusion, viability gating
- Compensation / unmixing verification
- Transformation — arcsinh scaling appropriate to the data modality
- Dimensionality reduction — UMAP via scanpy
- Clustering — Leiden or FlowSOM via Python wrapper
- Cluster annotation — marker expression heatmaps and biological interpretation
- Differential abundance — between-condition comparisons with appropriate statistical methods
- Reporting — a publication-quality multi-panel summary figure

Tools:
Python 3.11, FlowKit, scanpy, scikit-learn, pandas, NumPy, Matplotlib, Seaborn. Environment specified in environment.yml (added when the project begins).

Reproducibility:
Once the project is complete, this repository will include:
- A data download script
- A conda environment file
- Scripts numbered in execution order (01_qc.py, 02_transform.py, …)
- A single command (bash run_all.sh) to reproduce all figures

Background:
I work as a Resource Technologist at the University of Pennsylvania's Institute for Immunology and Immune Health. This portfolio represents independent computational work undertaken in preparation for graduate study in molecular biotechnology.

See also:

cytometry-r ; 
integrated-cytometry-analysis ; 
python-r-fundamentals

License:
MIT — see LICENSE file.
