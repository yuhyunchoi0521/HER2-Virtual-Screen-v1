# HER2-Virtual-Screen-v1
**Automated Bioavailable Drug Candidate Screening Pipeline**

## Project Overview
This project implements a virtual screening workflow for drug discovery using Python. It identifies potential lead compounds for **HER2-targeted therapies** (relevant in breast cancer research) by fetching real-world data from the **ChEMBL database** and applying pharmacokinetic filters.

## Scientific Framework: Lipinski’s Rule of Five
To assess the "drug-likeness" of molecules, this pipeline applies **Lipinski's Rule of Five**. This rule is a "rule of thumb" used to evaluate if a chemical compound has properties that would make it a likely orally active drug in humans.

**The Criteria used in this script:**
* **Molecular Weight (MW):** ≤ 500 Da
* **LogP (Hydrophobicity):** ≤ 5
* **H-Bond Donors:** ≤ 5
* **H-Bond Acceptors:** ≤ 10

*Reference: Lipinski, C. A., et al. (1997). Advanced Drug Delivery Reviews.*

## Tech Stack
- **ChEMBL API**: Used to query and download live biochemical data.
- **RDKit**: Used for molecular structure processing and descriptor calculation.
- **Pandas**: Used for data manipulation and tabular rendering.
- **Matplotlib**: Used for visualizing the distribution of results (Success/Failure rates).

## How it Works
1. **Data Acquisition**: Queries the ChEMBL API for molecules tested against the HER2 protein.
2. **Feature Extraction**: Converts SMILES strings into 2D molecular objects and calculates physical properties.
3. **Filtering**: Runs a logic-based check to see which molecules pass all four Lipinski criteria.
4. **Visualization**: Generates a summary pie chart and a detailed chemical property table.

## Key Learning
Through this project, I demonstrated:
- Connecting to professional bioinformatics APIs.
- Handling chemical data structures (SMILES).
- Applying Chemical Engineering principles to computational drug discovery.
- Data visualization for scientific decision-making.

---
*Developed as the start of my journey in merging Chemical Engineering with Computational Science.*
