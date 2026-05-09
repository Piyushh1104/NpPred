# NpPred: Prediction of Nuclear Proteins Using SVM and HMM Models

## Overview

NpPred is a computational method developed for predicting nuclear proteins using Support Vector Machine (SVM) and Hidden Markov Model (HMM) techniques.

The system combines sequence composition analysis and Pfam domain information to accurately distinguish nuclear proteins from non-nuclear proteins.

---

## Research Paper

**Title:** Prediction of nuclear proteins using SVM and HMM models

**Authors:**  
Manish Kumar and Gajendra P. S. Raghava

**Journal:** BMC Bioinformatics (2009)

**DOI:** https://doi.org/10.1186/1471-2105-10-22
https://doi.org/10.5281/zenodo.20099791
---

## Background

Nuclear proteins are involved in:

- Chromosomal maintenance
- Gene regulation
- RNA processing
- Nuclear transport
- Cellular homeostasis

Accurate prediction of nuclear proteins is important for:

- Functional annotation
- Proteome analysis
- Subcellular localization studies
- Computational biology

---

## Dataset Information

The study used a non-redundant dataset containing:

- 2710 nuclear proteins
- 7662 non-nuclear proteins

The dataset was extracted from Swiss-Prot release 40.41.

---

## Computational Approaches

The following approaches were implemented:

- Support Vector Machine (SVM)
- Hidden Markov Model (HMM)
- Hybrid SVM-HMM prediction

---

## Features Used

### Amino Acid Composition

Uses amino acid frequency information.

### Dipeptide Composition

Captures:

- Residue composition
- Local sequence order

### Split Amino Acid Composition (SAAC)

Protein sequences were divided into:

- N-terminal residues
- Remaining residues

Best results were obtained using:

- NT25+R composition model

---

## Important Residue Analysis

### Nuclear Proteins

Enriched residues:

- Lysine (K)
- Arginine (R)
- Glutamine (Q)
- Serine (S)
- Glutamic acid (E)

### Non-Nuclear Proteins

Higher abundance of:

- Leucine (L)
- Valine (V)
- Isoleucine (I)

---

## Best Performing Models

### Amino Acid Composition Model

- MCC: 0.59

### Dipeptide Composition Model

- Accuracy: 82.83%
- MCC: 0.61

### SAAC-Based Model

- Accuracy: 85.47%
- MCC: 0.66

### Hybrid SVM-HMM Model

- Accuracy: 94.61%
- MCC: 0.87

---

## Pfam Domain Analysis

The study identified:

- 558 exclusive nuclear domains
- 1197 exclusive non-nuclear domains
- 159 shared domains

A domain database named **NucPfam** was developed.

---

## Hybrid Prediction Strategy

### HMM-Based Prediction

- Exclusive nuclear domains predict nuclear proteins
- Exclusive non-nuclear domains predict non-nuclear proteins

### SVM-Based Prediction

Used when no exclusive domains are identified.

This hybrid strategy improved overall prediction accuracy.

---

## Benchmarking Results

NpPred outperformed several existing methods:

- BaCelLo
- LOCtree
- PredictNLS
- PSORT II
- NucPred

### Human Dataset Performance

| Method | Sensitivity |
|--------|-------------|
| NucPred | 0.63 |
| PredictNLS | 0.23 |
| LOCtree | 0.63 |
| BaCelLo | 0.61 |
| NpPred | 0.83 |

---

## Proteome Annotation

NpPred was used to analyze proteomes from:

- Saccharomyces cerevisiae
- Caenorhabditis elegans
- Drosophila melanogaster
- Mouse
- Human

### Predicted Nuclear Proteins

- Yeast: 31.51%
- Worm: 21.89%
- Fly: 26.31%
- Mouse: 25.72%
- Human: 24.95%

---

## Web Server

The NpPred server allows:

- Nuclear protein prediction
- Batch sequence submission
- Hybrid SVM-HMM prediction

Web Server:

http://www.imtech.res.in/raghava/nppred/

---

## Technologies Used

- SVM_light
- HMMER
- Pfam Database
- Perl
- CGI-Perl
- HTML

---

## Applications

NpPred can be used for:

- Nuclear protein prediction
- Functional genomics
- Proteome annotation
- Subcellular localization analysis
- Computational biology research

---

## Advantages

- High prediction accuracy
- Hybrid machine learning framework
- Domain-based prediction
- Large-scale proteome support

---

## Contact

### Prof. Gajendra P. S. Raghava

Department of Computational Biology  
Indraprastha Institute of Information Technology Delhi  
New Delhi, India

Email: raghava@iiitd.ac.in

---

## License

Creative Commons Attribution License

---

Generated from the uploaded NpPred research paper.
