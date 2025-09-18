# Disambiguator

Graph-Based Reference Disambiguation using legal case datasets.  
This repository implements a graph-based method to predict the correct legal reference in ambiguous contexts, based on co-occurrence statistics in past cases.

## 📌 Overview

This project builds a **co-occurrence graph of legal provisions** from a training dataset of judicial decisions and then uses **shortest-path distance on this graph** to infer the most likely legal reference in new evaluation examples.

**Main steps:**
1. Load and extract dataset (`dataset.zip`)
2. Construct a weighted undirected graph of co-occurring laws
3. Filter out weak edges and isolated nodes
4. Predict correct references for evaluation data by computing shortest-path distances to context laws

---

## ⚙️ Requirements

Python 3.9+ is recommended.  
Install dependencies:

```bash
pip install networkx
```
