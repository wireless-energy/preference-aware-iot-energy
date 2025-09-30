**Preference-aware Crowdsourcing of IoT Energy Services**

This repository contains the core implementation and evaluation code for the paper "Preference-aware Crowdsourcing of IoT Energy Services" (ICSOC 2025).
The code enables reproduction of the experiments described in Section 4 of the paper.

**Included Files:**

1 - PrefixSpan_Energy.ipynb in Code folder: This Jupyter Notebook runs the complete experimental pipeline used in the paper. It includes:
- Mining spatio-temporal mobility patterns using PrefixSpan
- Generating probabilistic pattern profiles
- Running provider-to-microcell allocation using various strategies (e.g., heuristics, GA, simulated annealing)
- Evaluating metrics such as Fulfillment Ratio, Reward Cost, and Energy Usage

2 - 0.5_7_probabilistic_patterns.csc in Dataset Folder: A sample output file showing mined mobility patterns using a minimum support of 0.5 across 7 venue categories. Each row corresponds to a provider's sequence of likely microcell visits across time intervals.

**Usage:**

- To run the full set of experiments:
- Open and execute all cells in the file PrefixSpan_Energy.ipynb using Jupyter Notebook or JupyterLab.
- The notebook performs all steps from data processing to allocation and metrics evaluation.
- The generated results may not match those shown in the evaluation section of the paper.

**Dataset Information:**
- The input mobility data is derived from the Foursquare dataset (New York City, April–June 2012).
- Only users with 50 or more days of history are used.
- Venue categories are mapped to microcells.
- Microcell demand ranges from 1000–2000 mAh.

**Output:**
- Evaluation metrics for each mode

## Citation

If you use this work, please cite:

```bibtex
@inproceedings{lakhdari2025preference,
  title={Preference-aware crowdsourcing of IoT energy services},
  author={Lakhdari, Abdallah and Abusafia, Amani and Lui, Shing Tai Tony and Bouguettaya, Athman},
  booktitle={International Conference on Service-Oriented Computing (ICSOC)},
  year={2025},
  organization={Springer}
}
