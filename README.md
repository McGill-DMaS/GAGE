# GAGE: Genetic Algorithm-based Graph Explainer for Malware Analysis

### Publication

M. Saqib, B. C. M. Fung, P. Charland, and A. Walenstein. GAGE: genetic algorithm-based graph explainer for malware analysis. In Proceedings of the 40th IEEE International Conference on Data Engineering (ICDE), pages 2258-2270, Utrecht, Netherlands: IEEE Computer Society, May 2024.

```plaintext
@inproceedings{SFCW24icde,
author = "M. Saqib and B. C. M. Fung and P. Charland and A. Walenstein",
title = "{GAGE}: Genetic Algorithm-based Graph Explainer for Malware Analysis",
booktitle = "Proc. of the 40th IEEE International Conference on Data Engineering (ICDE)",
pages = "2258-2270",
address = "Utrecht, Netherlands",
month = "May",
year = "2024",
publisher = "IEEE Computer Society",
}
```


## Overview

GAGE is a tool designed for malware analysis using genetic algorithms to explain graph structures. It integrates various components for constructing Canonical Executable Graphs (CEGs), training Graph Convolutional Networks (GCNs), and performing quantitative and robustness analysis.

## Repository Structure

### Main Scripts
- **CEG.py**: Constructs CEGs from disassembled binaries.
- **AED_training.py**: Trains embeddings for functions.
- **GA.py**: Implements the Genetic Algorithm-based Graph Explainer (GAGE) algorithm.

### GCN Related
- **GCN_AccuracyEnhancement.py**: Enhances the accuracy of the GCN model.
- **GCN_predict.py**: Uses the trained GCN model for predictions.
- **GCN_without_edgeFeatures.py**: GCN model without edge features.
- **GCN_withoutDuplicateNodes.py**: GCN model excluding duplicate nodes.

### GA for Experiments
- **GA_for_experiment_cfgexplainer.py**: GA script tailored for CFG explainer experiments.
- **GA_for_experiment_gage_cfg.py**: GA script configured for GAGE experiments.

### Quantitative and Robustness Analysis
- **quantitative_analysis.py**: Script for performing quantitative analysis on the generated graphs.
- **robustness_MMD_1perm.py**: Calculates robustness using the Minimum Mean Discrepancy (MMD) metric with one permutation.
- **robustness_subgraph.py**: Analyzes the robustness of subgraphs.
- **robustness_calculation.py**: General robustness calculation script.

### Plotting and Visualization
- **myplot/CFGExplainer.py**: Visualization for CFG explainer.
- **myplot_benign_4.py**: Plots benign samples.
- **myplot_bladabindi_emotet.py**: Plots Bladabindi and Emotet malware samples.
- **myplot_gex_3.py**: General plotting for experiments.
- **myplot_gex_4.py**: Additional plotting for benign samples.

### Utility Scripts
- **extract_subgraph.py**: Extracts subgraphs from the main graph.
- **blockFeatureGenerator.py**: Generates block features for the graphs.
- **utility.py**: General utility functions used across different scripts.


## Acknowledgments
GAGE was developed by Mohd Saqib under the supervision of Benjamin C. M. Fung, in the McGill Data Mining and Security Lab in Canada. It is distributed under the Creative Commons Attribution-NonCommercial 4.0 International License (for detail click [here!](https://github.com/McGill-DMaS/GAGE?tab=License-1-ov-file)). This research is supported by BlackBerry Limited (ALLRP 561035), Defence Research & Development Canada, and NSERC Alliance Grants (ALLRP 561035-20). Special thanks to Philippe Charland and Andrew Walenstein.

## Disclaimer
The software is provided as-is with no warranty or support. We do not take any responsibility for any damage, loss of income, or any problems you might experience from using our software. If you have questions, you are encouraged to consult the paper and the source code. If you find our software useful, please cite our paper above.

   
