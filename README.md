# LynFull_AllostericNetwork

This repository contains data and models supporting the manuscript:

**"Allosteric Coupling in Full-Length Lyn Kinase Revealed by Molecular Dynamics and Network Analysis"**  
Submitted to the Special Issue *Computational Approaches in Drug Design: Novel Methodologies and Applications*, International Journal of Molecular Sciences (IJMS).

---

## Overview

This work presents the first long-timescale molecular dynamics (MD) simulations of full-length Lyn kinase, spanning its SH3, SH2, and SH1 domains. Simulations were conducted across wildtype (WT) and mutant systems in apo and ligand-bound states. The study integrates structural modeling, correlation network analysis, and machine learning to uncover embedded allosteric hubs and interdomain coordination mechanisms.

---

## Repository Contents

- 🧬 `models/`:  
  Initial full-length Lyn kinase model (residues 60–502) generated via comparative modeling. Includes wildtype (WT) and all five cancer-associated mutants (K275A, E290D, E290K, I364L, I364N), provided in PDB format.

- 🧪 `input_coordinates/`:  
  Energy-minimized, solvated coordinate files used as input for production MD simulations. Separate files are provided for each WT and mutant system in both apo and holo (ATP-bound or dasatinib-bound) forms.

- 💥 `output_coordinates/`:  
  Representative structures (cluster medoids) derived from 6-μs MD simulations for all 13 systems. Files are provided in PDB format for downstream structural or network analysis.

- 🔗 `allosteric_hubs/`:  
  List of 44 dynamically embedded allosteric residues identified via network topology and interface-weighted scoring. Includes domain annotation, betweenness centrality, and integration module metrics (CSV format).

- 📊 `classification_features/`:  
  Pre-processed dataset containing 16 structural and dynamic features used in the Random Forest classifier. Features include interdomain distances, angles, and key interaction metrics (CSV format).

---  
 
## 📚 Citation

If you use this dataset, code, or model in your research, please cite the associated publication:  

Rabipour, M.; Hassenrück, F.; Pallaske, E.; Röhrig, F.; Hallek, M.; Alvarez-Idaboy, J.R.; Kramer, O.; Rebollido-Rios, R.  
**Allosteric Coupling in Full-Length Lyn Kinase Revealed by Molecular Dynamics and Network Analysis.**  
*International Journal of Molecular Sciences.* 2025, 26, 5835. https://doi.org/10.3390/ijms26125835  

Additionally, please cite this repository:  
Rebollido-Ríos R. *et al.* (2025). **Lyn Kinase Allosteric Coupling [Code and Data].** Zenodo.  
https://doi.org/10.5281/zenodo.

---

## ✉️ Contact

For questions, feedback, or requests for additional data, feel free to reach out to:

- **Rocio Rebollido-Rios:** [rocio.rebollido-rios@uni-koeln.de](mailto:rocio.rebollido-rios@uni-koeln.de)  
- **Mina Rabipour:** [mina.rabipour@uk-koeln.de](mailto:mina.rabipour@uk-koeln.de)


© 2025 Rebollido-Rios Lab. Released for academic research purposes.
