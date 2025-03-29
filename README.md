# ChEMBL Compound Data Acquisition for SARS-CoV-2 Mpro
🔬 *Bioactivity Data Extraction for COVID-19 Drug Discovery*

## Project Overview
This project retrieves and processes bioactivity data from the ChEMBL database for **SARS-CoV-2 Main Protease (Mpro)**, a crucial viral enzyme and therapeutic target. The dataset includes:
- **Bioactivity measurements**: IC50 and Ki values
- **Derived metrics**: pIC50 and pKi scores
- **Compound structures**: SMILES representations
- **Molecular properties**: For cheminformatics analysis

## Key Steps
1. **Data Acquisition**
   - Connect to ChEMBL database (Version 27)
   - Retrieve target data for SARS-CoV-2 Mpro (`CHEMBL4523582`)
   - Fetch bioactivity data (IC50 and Ki values)

2. **Data Processing**
   - Calculate pIC50 and pKi values
   - Standardize units and filter compounds
   - Merge bioactivity and compound data

3. **Output**
   - Visualize potent compounds
   - Freeze dataset to ChEMBL 27 for reproducibility
   - Export final dataset (`MPro_compounds_200325.csv`)

## Dataset Features
| Feature | Description |
|---------|-------------|
| **Target** | SARS-CoV-2 Main Protease (Mpro) |
| **Bioactivity** | IC50, Ki, pIC50, pKi values |
| **Structures** | Canonical SMILES |
| **Source** | [ChEMBL Database](https://www.ebi.ac.uk/chembl/) (Version 27) |

## Requirements
- Python 3.x
- Required packages:
  ```bash
  pip install pandas numpy rdkit chembl_webresource_client tqdm# Covid-Mpro-ChEMBL
ChEMBL-derived bioactivity data for SARS-CoV-2 Main Protease (MPro) inhibitors. Includes IC50/pIC50 and Ki/pKI values, compound structures, and cheminformatics analysis
