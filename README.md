# Identification and Elucidation of Therapeutic Targets in Nasopharyngeal Carcinoma

### A Computational Bioinformatics Study

[![Publication](https://img.shields.io/badge/Published-2026-blue)](https://doi.org/10.32350/cto.61.03)
[![DOI](https://img.shields.io/badge/DOI-10.32350%2Fcto.61.03-blue)](https://doi.org/10.32350/cto.61.03)

> Computational investigation of transcriptomic alterations in nasopharyngeal carcinoma using differential expression, pathway enrichment, protein-protein interaction networks, and hub-gene analysis.
>
> ## 📌 Project Overview

Nasopharyngeal carcinoma (NPC) is a malignant tumor with complex molecular characteristics. This study used publicly available gene-expression data to identify differentially expressed genes, enriched biological pathways, protein-protein interaction networks, and potential hub genes associated with NPC.

The analysis was performed using the **GEO dataset GSE53819**, containing **18 NPC tumor samples and 18 normal nasopharyngeal tissue samples**. The study integrated differential expression analysis, pathway enrichment, and PPI network analysis to prioritize candidate therapeutic targets.

## 📊 Dataset

**GEO accession:** [GSE53819](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE53819)

The dataset contains **36 samples**:

- **18 primary nasopharyngeal carcinoma (NPC) tumor samples**
- **18 normal nasopharyngeal tissue samples**

**Platform:** Agilent-014850 Whole Human Genome Microarray 4x44K, **GPL6480**

The dataset was obtained from the publicly accessible **Gene Expression Omnibus (GEO)** database and was used for transcriptomic analysis of NPC. :contentReference[oaicite:0]{index=0}

## 🔬 Analysis Methods

The computational workflow consisted of four main stages:

1. **Differential Expression Analysis**
   - GEO2R was used to identify differentially expressed genes.
   - Genes were filtered using adjusted *p* ≤ 0.05 and a final `|logFC| > 1.5` criterion.

2. **Functional & Pathway Enrichment**
   - Gene Ontology (GO) and KEGG pathway enrichment were performed.
   - Consensus Pathway Analysis (CPA) integrated Wilcoxon, FGSEA, and Kolmogorov-Smirnov tests.
   - DAVID was used for pathway validation.

3. **Protein-Protein Interaction Network**
   - STRING was used to construct the PPI network.
   - Interactions below a confidence score of 0.4 were excluded.
   - Cytoscape was used for network visualization.

4. **Hub Gene Identification**
   - CytoHubba was used within Cytoscape.
   - The Maximal Clique Centrality (MCC) method was used to prioritize hub genes.
  
   - ## 📈 Key Results

- **11,331** differentially expressed genes were initially identified.
- After filtering, **250 high-confidence DEGs** remained, including **213 upregulated** and **37 downregulated** genes.
- **11 KEGG pathways** showed significant enrichment.
- The PPI network contained **119 nodes and 5,040 edges**.
- **10 hub genes** were prioritized using the MCC method:

`IL1B · FN1 · CXCL8 · CD19 · CSF2 · CXCL12 · IFNG · COL1A1 · CXCL10 · FCGR3A`

### Key Biological Findings

Two major network modules were highlighted:

**Inflammatory cytokine–chemokine axis**  
`IL1B → CXCL8 → CXCL12`

**ECM remodeling axis**  
`FN1 → COL1A1`

Together, these findings suggest coordinated inflammatory and extracellular-matrix processes associated with NPC progression and tumor immune regulation.

## 📄 Publication

**Wajeeha Urooj**, Misbah Jamil, Zaneb Rehman, Aamra Sohail, Sidra Majaz, Ashfaq Ahmad.

**Identification and Elucidation of Therapeutic Targets in Nasopharyngeal Carcinoma: A Computational Approach**

*Current Trends in OMICS*, 6(1), 40–63, 2026.

[![DOI](https://img.shields.io/badge/DOI-10.32350%2Fcto.61.03-blue)](https://doi.org/10.32350/cto.61.03)

📖 [Read the published article](https://journals.umt.edu.pk/index.php/CTO/article/view/7696)
