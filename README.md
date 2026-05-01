# GGR376H5 — CaféTO Spatial Analysis

**Course:** GGR376H5 — Geographic Information Science II  
**Term:** Winter 2025 · Group 15  
**Institution:** University of Toronto Mississauga

---

## Overview

This is the final project for GGR376H5, a spatial analysis examining whether CaféTO outdoor café permit density is spatially associated with neighbourhood median household income across Toronto's 158 neighbourhoods.

The project applies core concepts from the course — spatial joins, autocorrelation, and regionalization — to a real-world equity question: are outdoor dining spaces disproportionately concentrated in wealthier neighbourhoods?

---

## Research Question

> Is the distribution of CaféTO outdoor café permits spatially correlated with neighbourhood median household income in Toronto?

---

## Methods & Concepts Applied

| Technique | Purpose |
|-----------|---------|
| GeoPandas spatial join | Link permit point locations to neighbourhood polygons |
| Choropleth mapping | Visualise permit density and income by neighbourhood |
| Global Moran's I | Test for overall spatial autocorrelation (I = 0.5998, p = 0.001) |
| Local LISA clustering | Identify significant High-High / Low-Low spatial clusters |
| SKATER regionalization | Build spatially-contiguous clusters (5 regions) |

**Key finding:** Strong positive spatial autocorrelation (I ≈ 0.60) — CaféTO permits cluster in higher-income neighbourhoods, particularly in the downtown core.

---

## Data Sources

All data fetched directly from public APIs (no local files required):

- **Toronto Neighbourhood Boundaries** — City of Toronto Open Data  
- **CaféTO Permit Locations** — City of Toronto Open Data  
- **2021 Census Neighbourhood Profiles** — City of Toronto Open Data

---

## Files

| File | Description |
|------|-------------|
| `GGR376_Group15_Proposal_Analysis_.ipynb` | Main analysis notebook (GeoPandas, PySAL, SKATER) |
| `Project Proposal-group15.docx` | Original project proposal document |

---

## How to Run

Open the notebook in Google Colab — all data is fetched directly from Toronto Open Data URLs, so no local setup is needed.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1GHHWURdU2tpAGdzpULWZb1XOAVpZsI3m)
