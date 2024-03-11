# V2O5 Quasiparticle and Excitonic Research

This repository contains data and supporting files for the research paper "Quasiparticle band structure and excitonic optical response in V2O5 bulk and monolayer" by Claudio Garcia, Santosh Kumar Radha, Swagata Acharya, and Walter R. L. Lambrecht.  [arXiv link to the paper]

**Repository Structure**

* **agr:** Contains .agr files for visualization with xmgrace (https://plasma-gate.weizmann.ac.il/Grace/). Correlates to figures 3, 4, 7, 8, and 9 in the paper.
* **vesta:** Contains .vesta files for visualization with VESTA (https://jp-minerals.org/vesta/en/). Supports Fig. 5, offering interactive 3D exploration of the structure and exciton wavefunction data.
* **bnds-blk/bnds-mono:** Ascii files containing band structure data (number of bands, Fermi level, k-point labels, energy eigenvalues) for figures 2 and 6. Includes DFT GGA-PBE, QSGW-RPA, and QSGW (with ladder diagrams) calculations. See https://www.questaal.org/docs/input/data_format/#bnds-file for format details and https://www.questaal.org/docs/misc/plbnds/ for visualization.
* **bnds-k:** Contains exciton band weight data (Fig. 5 a-c) in .h5 format. Refer to https://www.questaal.org/docs/code/userguide/ for details on usage.
* **ctrl.v2o5** and **site.v2o5:**  Input files for generating all data.
* **.rst**, **.syml**, **.sigm:** Restart and self-energy files for rapid regeneration of results.

**Using the Data**

1. **Visualization:** 
   * Use xmgrace with provided .agr files
   * Employ VESTA with .vesta files for 3D structural and exciton wavefunction exploration.

2. **Band Structure Analysis:**
   * Load ascii files in data analysis software of your choice. See provided links for format and visualization guidance.

3. **Exciton Band Weights:**
   * Use the instructions at https://www.questaal.org/docs/code/userguide/ to integrate weights over energy windows and enhance band plots.

**Reproducibility**

The provided input files, restart data, and self-energy files allow for the quick and complete regeneration of the presented results.

**Contact and Collaboration**

* For questions or feedback on the data or research, please contact the authors via walter.lambrecht@case.edu. 
* We welcome collaborations and contributions to further this research.