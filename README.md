# Patent Fuzzy Intelligence Analysis

Replication code and dataset for the paper:

**"Fuzzy Logic Assessment of Commercial and Academic Impact in 
Emerging Economy Patent Portfolios: Evidence from Colombia, 
Brazil, Vietnam, and Malaysia"**

Submitted to ICECCME 2026 - 6th International Conference on 
Electrical, Computer, Communications and Mechatronics Engineering.
Bali, Indonesia, 15-17 October 2026.

---

## Dataset and Replication Files

Full dataset including raw patent CSV files and replication 
code is permanently archived at:

**Zenodo DOI:** https://doi.org/10.5281/zenodo.20112899

---

## Data Sources

Patent data was retrieved from **Lens.org** (https://www.lens.org),
an open-access patent database. Records were extracted using the
applicant country filter for each country:

| Country  | Filter         | Records |
|----------|----------------|---------|
| Brazil   | applicant = BR | 211,181 |
| Malaysia | applicant = MY |  35,200 |
| Colombia | applicant = CO |  14,100 |
| Vietnam  | applicant = VN |   4,523 |
| **Total**|                |**265,004**|

Publication date range: 2020-01-01 to 2025-12-31

Macroeconomic indicators were retrieved from the 
**World Bank Open Data API** (https://data.worldbank.org)
using the following codes:

- `NY.GDP.PCAP.CD` — GDP per capita (USD)
- `IP.PAT.RESD` — Patent applications by residents
- `GB.XPD.RSDV.GD.ZS` — R&D expenditure (% of GDP)
- `NY.GDP.MKTP.KD.ZG` — GDP growth rate (%)

---

## Repository Structure
patent-fuzzy-intelligence/
├── README.md
├── patent_fuzzy_analysis.ipynb   # Main analysis notebook
├── references.bib                # BibTeX references
├── fig1_scores.png               # CIP and AIP scores by country
├── fig2_scatter.png              # Portfolio positioning plot
└── fig3_cpc.png                  # CPC technological specialization

---

## Requirements
Python 3.x
scikit-fuzzy
pandas
numpy
matplotlib
requests

Install with:
pip install scikit-fuzzy pandas numpy matplotlib requests

---

## Usage

1. Download the full dataset from Zenodo:
   https://doi.org/10.5281/zenodo.20112899
2. Place the CSV files in the same directory as the notebook
3. Open `patent_fuzzy_analysis.ipynb` in Google Colab or Jupyter
4. Run all cells in order

---

## Results

| Country  | CIP   | AIP   |
|----------|-------|-------|
| Colombia | 5.384 | 4.517 |
| Brazil   | 5.023 | 4.518 |
| Vietnam  | 4.976 | 5.378 |
| Malaysia | 5.013 | 4.518 |

CIP = Commercial Impact Potential (0-10)
AIP = Academic Impact Potential (0-10)

---

## License

This work is licensed under 
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

---

## Citation

If you use this code or dataset, please cite:
[Authors]. (2026). Fuzzy Logic Assessment of Commercial and
Academic Impact in Emerging Economy Patent Portfolios: Evidence
from Colombia, Brazil, Vietnam, and Malaysia.
ICECCME 2026. https://doi.org/10.5281/zenodo.20112899
