# Reproducibility package for Galactic-plane alignment analysis of open-cluster shapes in Gaia DR3

Version: **1.0.0**  
Release date: **2026-10-28**

This archive contains analysis code, machine-readable derived tables, vector figures,
figure-generation code, environment specifications, and provenance material supporting
the study:

**Persistent Galactic-Plane Alignment of Open-Cluster Shapes in Gaia DR3: Matched Age Controls, Radial Tests, and Orbital Constraints**

## Deliberate exclusion

The article manuscript, article PDF, LaTeX source, bibliography, cover letter, and
submission correspondence are **not included**.

## Directory structure

- `code/core_pipeline/` — main catalogue, morphology, alignment, matched-control,
  inner-region, age-extension, and orbital calculations.
- `code/sensitivity_analyses/` — estimator, projection, selection/environment,
  local-gradient, dependence, ceiling, latitude, geometry, and exact block analyses.
- `code/figure_generation/matlab/` — MATLAB sources for the seven deposited figures.
- `figures/vector_pdf/` — final vector PDFs in article figure order.
- `tables/` — machine-readable CSV result tables.
- `results/` — compact machine-readable headline metrics.
- `metadata/` — Zenodo-ready metadata, creators, data sources, licenses, and indices.
- `provenance/` — source-archive hashes and sample identity hashes.
- `tools/` — package integrity and DOI utilities.

## Environment

Create a Conda environment with `environment.yml`, or install `requirements.txt`.
MATLAB R2020a or later is recommended for the figure scripts.

## Integrity

Run:

`python tools/verify_package.py`

## DOI

No DOI is fabricated in this archive. Reserve a DOI in Zenodo, then use:

`python tools/set_zenodo_doi.py 10.5281/zenodo.XXXXXXX`

After changing metadata, rebuild `MANIFEST.csv` and `SHA256SUMS.txt`.

## Licensing

Code: MIT.  
Deposited derived tables and vector figures: CC BY 4.0.  
See `metadata/LICENSES.md`.
