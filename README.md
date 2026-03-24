# 🎬 TemporalFairRecSysFramework

Self-contained Jupyter notebooks for **knowledge graph–based recommender systems** on **MovieLens 1M**, with **temporal learning** and **fairness/exposure bias mitigation**.

Think of it as your one-stop playground for trying out multiple recommender models without worrying about preprocessing headaches.

---

## 📂 Repository Layout

| 📓 Notebook                            | 🔍 Purpose                                                      |
| -------------------------------------- | --------------------------------------------------------------- |
| `data-preprocessing.ipynb`             | General preprocessing reference (not needed for running models) |
| `baseline-*.ipynb`                     | Baseline models with built-in preprocessing                     |
| `temporal-*.ipynb`                     | Temporal models (time-aware versions)                           |
| `final-*.ipynb`, `pinsage-final.ipynb` | Final models with fairness & exposure mitigation                |
| `hyperparam-test-for-kgcn.ipynb`       | KGCN hyperparameter tuning experiments                          |

> ⚠️ Every notebook already includes preprocessing for that specific model, so you **don’t need to run `data-preprocessing.ipynb`**.

---

## 🚀 How to Use

1. Clone the repo:

```bash
git clone https://github.com/Sajith-Santhosh/TemporalFairRecSysFramework.git
```

2. Open **any notebook** in Jupyter, Colab, or Kaggle.
3. Run all cells top-to-bottom.
4. Metrics are printed directly in outputs (no plots saved).

---

## 🧩 Models Covered

| Model           | 🔹 Description                                             |
| --------------- | ---------------------------------------------------------- |
| DistMult        | Knowledge graph embedding                                  |
| TransH          | Knowledge graph embedding with relation hyperplanes        |
| KGCN            | Knowledge graph convolutional network                      |
| LightGCN        | Simplified GCN for collaborative filtering                 |
| PinSage         | Graph-based recommendations with random walks              |
| Temporal / Fair | Variants with temporal smoothing & fairness regularization |

---

## 📊 Evaluation Metrics

| Metric                      | Meaning                                    |
| --------------------------- | ------------------------------------------ |
| ✅ Recall                    | How many relevant items got recommended    |
| 🎯 NDCG                     | Ranking quality                            |
| ⚖️ EO (Equal Opportunity)   | Fairness across user slices                |
| 🏛️ DP (Demographic Parity) | Exposure fairness across groups            |
| 🌈 Gini                     | Concentration / diversity of item exposure |

All metrics are printed inline in the notebook outputs.

---

## 📚 References

| Model    | Paper                                                                                                  |
| -------- | ------------------------------------------------------------------------------------------------------ |
| DistMult | Yang et al., *"Embedding Entities and Relations for Learning and Inference in Knowledge Bases"* (2015) |
| TransH   | Wang et al., *"Knowledge Graph Embedding by Translating on Hyperplanes"* (2014)                        |
| KGCN     | Wang et al., *"KGAT: Knowledge Graph Attention Network for Recommendation"* (2019)                     |
| LightGCN | He et al., *"LightGCN: Simplifying and Powering Graph Convolution Network for Recommendation"* (2020)  |
| PinSage  | Ying et al., *"Graph Convolutional Neural Networks for Web-Scale Recommender Systems"* (2018)          |

---

## 🏁 MIT License

