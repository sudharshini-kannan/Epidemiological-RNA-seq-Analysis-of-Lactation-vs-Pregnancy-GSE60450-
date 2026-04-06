# 🧬 Epidemiological RNA-seq Analysis (GSE60450)

## 📌 Project Overview

This project performs differential gene expression analysis on RNA-seq data to compare **pregnancy vs lactation** conditions using dataset **GSE60450**.

The goal is to identify genes that are significantly upregulated or downregulated between these two physiological states.

---

## 🎯 Objectives

* Process RNA-seq count data
* Perform differential expression analysis
* Visualize gene expression patterns
* Interpret biological differences between conditions

---

## 📂 Dataset

* **Source:** GEO (GSE60450)
* **Samples:** 12

  * Pregnancy: 6
  * Lactation: 6

---

## 🛠️ Tools & Technologies

* R
* DESeq2
* pheatmap
* ggplot2

---

## 🔬 Methodology

### 1. Data Preprocessing

* Loaded gene count data
* Removed non-expression columns (e.g., gene length)
* Cleaned and matched sample names with metadata

### 2. Differential Expression Analysis

* Created DESeq2 dataset
* Normalized counts
* Identified significantly expressed genes

### 3. Visualization

* Volcano Plot → significance vs fold change
* Heatmap → top 20 genes
* PCA Plot → sample clustering

---

## 📊 Results

### 🔹 Differential Expression

* Identified significant genes (p-value < 0.05)
* Both upregulated and downregulated genes observed

### 🔹 PCA Analysis

* Clear separation between pregnancy and lactation samples
* Indicates strong biological differences

### 🔹 Heatmap

* Top genes show distinct expression patterns between conditions

---

## 🧠 Biological Interpretation

The analysis reveals that gene expression profiles differ significantly between pregnancy and lactation.
These differences reflect physiological and metabolic adaptations associated with each stage.

---

## 📁 Project Structure

```
epidemiological-rnaseq-analysis/
│── data/
│   ├── GSE60450_Lactation-GenewiseCounts.txt
│   ├── metadata.csv
│
│── scripts/
│   ├── analysis.R
│
│── results/
│   ├── plots/
│
│── README.md
```

---

## 🚀 How to Run

```bash
# Open R
R
```

```r
# Load libraries
library(DESeq2)
library(pheatmap)

# Run analysis script
source("scripts/analysis.R")
```

---

## 📌 Key Learnings

* Handling real-world RNA-seq data
* Debugging sample mismatches
* Performing differential expression analysis
* Visualizing biological insights

---

## 💼 Author

**Sudharshini Kannan**
Bioinformatics & Biotechnology Enthusiast

---

## ⭐ Future Improvements

* Functional enrichment analysis (GO/KEGG)
* Pathway analysis
* Integration with clinical metadata
