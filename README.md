# Metagenomics Homework 2: Environmental Microbiome Exploratory Analysis
---

## Project Structure

```
metagenomics_hw_2/
├── README.md                                          # This file
├── exploratory_analysis.ipynb                         # Main analysis notebook
├── urban_microbiome_research.ipynb                    # Related research notebook
├── input/
│   ├── environmental_core_wide_2026-02-01.tsv         # Metadata (16,994 samples)
│   └── environmental_metaphlan4_species_2026-02-01.tsv # Species abundance data
└── output/
```

---

## Dataset Description

### Input Files

#### 1. **environmental_core_wide_2026-02-01.tsv** (Metadata)
- **Format:** Tab-separated values
- **Samples:** 16,994 environmental samples
- **Metadata variables:** ~100+ fields organized into categories:
  - **Identifiers:** sample_alias, study_code, sample ID
  - **Geographic:** longitude, latitude, geographic_location
  - **Temporal:** collection_date, sampling year/season
  - **Environmental:** biome classification, habitat, material type
  - **Technical:** sequencing platform, filtration parameters
  - **Physicochemical:** pH, temperature, elevation, depth, precipitation

#### 2. **environmental_metaphlan4_species_2026-02-01.tsv** (Species Abundance)
- **Format:** Long format (sample × species pairs)
- **Rows:** 1,653,440 (after duplicate aggregation)
- **Unique samples:** 16,994
- **Unique species:** 25,003
- **Values:** Relative abundance per species per sample
- **Normalization:** Abundances sum to ~1.0 per sample

---

## Usage

### Running the Analysis

1. **Prerequisites:**
   ```bash
   pip install pandas numpy matplotlib seaborn scipy
   ```

2. **Execute notebook:**
   ```bash
   jupyter notebook exploratory_analysis.ipynb
   ```

3. **Run all cells** to generate complete analysis and outputs


4. **Execute notebook:**
   ```bash
   jupyter notebook urban_microbiome_research.ipynb
   ```

5. **Run all cells** to generate complete analysis and outputs