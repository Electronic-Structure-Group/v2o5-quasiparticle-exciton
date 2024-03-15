# Quasiparticle Band Structure and Excitonic Optical Response in V2O5 Bulk and Monolayer

This GitHub repository hosts the data files and related information for the research paper titled "Quasiparticle band structure and excitonic optical response in V2O5 bulk and monolayer," authored by Claudio Garcia, Santosh Kumar Radha, Swagata Acharya, and Walter R. L. Lambrecht, available on 	arXiv:2403.05473

## Repository Structure

The repository is structured to provide easy access to the data files used in the figures of the paper. Below is a guide to the contents and organization:

### 1. Grace Files (Folder: `agr`)
- **Description**: Contains `.agr` and eps-plot.txt column structured data files for use with [XMGRACE](https://plasma-gate.weizmann.ac.il/Grace/).
- **Figures Covered**: 3, 4, 7, 8, 9.
- **Contents**: Datasets corresponding to the mentioned figures.

### 2. VESTA Files (Folder: `vesta`)
- **Description**: Includes `.vesta` and zip compressed .xsf files for visualization with [VESTA](https://jp-minerals.org/vesta/en/).
- **Figure Covered**: 5, 10 
- **Features**: Enables users to explore the structure and exciton wavefunction data from various angles and adjust isosurface values for exciton distributions.

### 3. Band Structure Data (Folders: `bnds-blk` and `bnds-mono`)
- **Description**: Contains ASCII files with band structure data relevant to figures 2 and 6.
- **Data Format**: Information on the number of bands, Fermi level, k-point labels, and energy eigenvalues. Details at [Questaal Data Format](https://www.questaal.org/docs/input/data_format/#bnds-file).

```line 1: number of bands, Fermi level, k-point labels
line 2: number of points long first line
line 3: k-point coordinates in units 2pi/a  with a the lattice constant
lines 4 -40: energy eigenvalues  in Rydberg
line 5: next k-point followed by bands etc.
until end of line.
```

- **Visualization**: Data can be visualized using [Questaal's plbnds tool](https://www.questaal.org/docs/misc/plbnds/).
- **Files Included**: `bnds.gga`, `bnds.ldr`, `bnds.rpa` (representing different computational approximations).



### 4. Meta Data 
- **Description**: Provides the fundamental input files (`ctrl.v2o5` and `site.v2o5`) needed to generate all the dataset, alongside `.rst`, `syml`, and `sigm` files for the self-consistent potential restart data and the self-energy files.
- **Organization**: Data is arranged in subfolders for the bulk and various `c` values, facilitating quick regeneration of the results.

## Additional Information

For more details on the paper and the corresponding research findings, please refer to the [arXiv publication](#).

This repository aims to support the reproducibility of our research by providing comprehensive datasets and tools necessary for analysis. We encourage the use of these resources in academic and research settings.
