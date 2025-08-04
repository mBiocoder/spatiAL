# spatiAL: Discovering genetic determinants of subcellular spatial biology by active learning

This repository contains the code and experiments conducted for my Master's thesis: **“Discovering genetic determinants of subcellular spatial biology by active learning
”**, where I developed and evaluated a deep learning framework for analyzing SPARCS-based imaging data to uncover novel insights into autophagy.

---

## Abstract

The rapid expansion of high-throughput genomic technologies, such as CRISPR-based genetic screens, has revolutionized our ability to explore cellular processes at scale. This thesis integrates deep learning with high-content imaging to enhance our understanding of **autophagy**—a key mechanism for cellular homeostasis. Using the **SPARCS** platform for spatially resolved CRISPR screening, I developed a **multiclass-autophagy classifier**, compared various deep learning models (e.g., ConvNeXt variants), and explored **semi-supervised** and **active learning** approaches for label-efficient phenotyping. The models were validated against a biologically curated autophagy classifier, showing promise in detecting subtle phenotypes and novel biological patterns.

---

## Repository Structure

This repo is organized into several subdirectories, each corresponding to a major methodological or experimental component of the thesis:

| Folder              | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `General/`          | Utility scripts, installation, data overview, data loaders, and subset creation and preprocessing code. |
| `Supervised/`       | Supervised training workflows, including baseline ConvNeXt models and multiclass classifier training across various Cases. |
| `Semisupervised/`   | Experiments with semi-supervised learning using partially labeled datasets with ConvNeXt and embedding distance calculations. |
| `Active_learning/`  | Simulated active learning loop for efficient annotation using ConvNeXt. |
| `Ensembling/`       | Ensemble models for autophagy multiclass classifer on various seeds. |
| `timecourse_images/`| Timecourse images of wilttype (WT) and EI24 KO. |

---

## Key Contributions

- Developed a **multiclass deep learning classifier** for autophagy phenotypes using SPARCS data.
- Leveraged **ConvNeXt** and compared with fine-tuned and baseline variants.
- Integrated **semi-supervised learning** to utilize unlabeled data and improve generalization.
- Designed a **simulated active learning loop** to reduce annotation burden.
- Emphasized **model interpretability and uncertainty estimation** to enhance biological insight.
- Validated using a **biologically validated autophagy 2↔1 classifier** and gRNA enrichment analysis.

