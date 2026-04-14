# UltraGCN

This repository is part of **RecZoo**, a curated model zoo for recommendation tasks.  
In this fork, **our team focuses exclusively on implementing and experimenting with UltraGCN**.

> **CIKM 2021** — Kelong Mao, Jieming Zhu, Xi Xiao, Biao Lu, Zhaowei Wang, Xiuqiang He.  
> **UltraGCN: Ultra Simplification of Graph Convolutional Networks for Recommendation**  
> Paper: https://arxiv.org/pdf/2110.15114.pdf

- Original UltraGCN implementation: https://github.com/RecZoo/UltraGCN

---

## 📌 Overview

**UltraGCN** is an advanced simplification of Graph Convolutional Networks for recommendation.  
Instead of performing explicit graph convolutions, UltraGCN **reformulates the message passing mechanism into a constraint-based loss**, significantly improving:

- Training efficiency
- Scalability to large datasets
- Recommendation performance

This makes UltraGCN highly suitable for large-scale collaborative filtering tasks.

Our fork focuses on:

- Clean and reproducible experiments
- Structured experiment tracking
- Running and validating experiments on Google Colab
- Understanding UltraGCN behavior across datasets

Although RecZoo contains many recommendation models across matching, ranking, pretraining, and personalization tasks, **this repository only implements and evaluates:**

| No | Model     | Publication |
|:--:|-----------|-------------|
| 1  | **UltraGCN** | Kelong Mao et al., *UltraGCN: Ultra Simplification of Graph Convolutional Networks for Recommendation*, CIKM 2021 |

---

## 📂 Supported Datasets

This implementation supports four widely used benchmark datasets and one custom dataset prepared by our team:

| Dataset       | Description                                  |
|---------------|----------------------------------------------|
| **Gowalla**   | Location-based social network check-ins      |
| **Yelp2018**  | Business reviews and user ratings            |
| **Amazon-Book** | Book purchase and rating records          |
| **MovieLens1M** | Movie rating dataset                      |
| **GitStar**   | Self-crawled dataset based on GitHub stars  |


---

## 🧪 Experiments

We conducted careful experiments using the PyTorch version of UltraGCN.  
All experimental runs, logs, and metric tracking are stored in the `exp/` directory as Jupyter notebooks.

To ensure transparency and academic integrity, we provide public Google Drive links containing:

- The source code from this repository that we uploaded on Google Drive to mount for experiment running
- Execution logs
- Output results
- Saved checkpoints and metrics

These materials serve as **self-proof** that all experiments were conducted by our team on **Google Colab**, without reusing results from external sources. Accessing each link will lead to a folder with three folder LightGCN, UltraGCN and LayerGCN. The source code for this repository is uploaded inside the UltraGCN folder for all three links

**Note: The souce in the UltraGCN folder inside each drive link is upload from the `matching/gnn/UltraGCN` path of this repository**

### Environment

- Google Colab (GPU)
- PyTorch implementation
- Multiple reruns to verify consistency

### Experiment Notebooks

| Notebook             | Description                        | Link |
|----------------------|------------------------------------|------|
| `ultra_exp`       | Initial experimental run           | https://drive.google.com/drive/folders/1Iq_NvTZkTy8MYP-0DPvymDHFO2nDsFK_?usp=drive_link |
| `ultra_rerun_1`   | Run the second time        | https://drive.google.com/drive/folders/1l93GDNQzRcL9pg4eR6vriTOxrzcUY_G5?usp=drive_link |
| `ultra_rerun_2`   | Run the third time | https://drive.google.com/drive/folders/12VtE9kucBlikg8x8cVtrnuwBRTTBC68d?usp=drive_link |

These notebooks contain:

- Training configurations
- Evaluation metrics (Recall, NDCG, etc.)
- Result comparisons across runs

---

## 🎯 Purpose of This Fork

This fork was created for:

- Academic experimentation with UltraGCN
- Reproducible research
- Understanding constraint-based graph learning for recommendation
- Structured documentation of experimental results

---

## 🙏 Acknowledgements

We sincerely thank the authors of UltraGCN and the RecZoo project for making their work publicly available.

If you use this codebase, please consider citing the original paper.