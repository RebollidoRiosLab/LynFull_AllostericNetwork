# LynFull_AllostericNetwork

This repository contains data and models supporting the manuscript:

**"Allosteric Coupling in Full-Length Lyn Kinase Revealed by Molecular Dynamics and Network Analysis"**  
Submitted to the Special Issue *Computational Approaches in Drug Design: Novel Methodologies and Applications*, International Journal of Molecular Sciences (IJMS).

## Overview

This work presents the first long-timescale molecular dynamics (MD) investigation of full-length Lyn kinase, spanning its SH3, SH2, and SH1 domains. Simulations were conducted across wildtype (WT) and mutant systems in apo and ligand-bound states. The study integrates structural modeling, correlation network analysis, and machine learning to uncover embedded allosteric hubs and interdomain coordination mechanisms.

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

## Citation

If you use this dataset or model in your research, please cite the associated publication once available.

## Contact

For questions or requests for additional simulation data:
📧 Rocio Rebollido-Rios — *rocio.rebollido-rios@uni-koeln.de*

---

© 2025 Rebollido-Rios Lab. Released for academic research purposes.
