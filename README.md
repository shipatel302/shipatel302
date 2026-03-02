# Shivani Patel

<div align="center">

### I turn biological chaos into actionable insight.

*Single cells. Whole genomes. Drug targets. Clinical records.*
*From raw data to decisions — end to end.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-shivanip99-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/shivanip99)
[![Email](https://img.shields.io/badge/Email-shivanip8369@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shivanip8369@gmail.com)
[![University](https://img.shields.io/badge/M.S._Bioinformatics-University_of_Delaware-003087?style=for-the-badge)](https://www.udel.edu)

</div>

---

## The Short Version

> I am a **bioinformatician, data scientist, and statistical modeler** with 4+ years of experience.
> I build things that scale, run analyses that hold up under scrutiny,
> and communicate findings that people actually understand and use.

**The data I work with:** single-cell RNA-seq · bulk RNA-seq · whole genome & exome · proteomics · HTS compound screens · clinical records · multi-omics

**The problems I solve:** disease subtype classification · drug target identification · somatic variant detection · pathway dysregulation · compound hit prioritization · pipeline bottlenecks

**The standard I hold:** reproducible · statistically rigorous · biologically interpretable · production-ready

---

## What I Actually Do

```
Raw Data                         Insight
────────                         ───────
FASTQ files          ──▶   QC → Alignment → Variant Calling → Annotation
scRNA-seq counts     ──▶   Normalization → Clustering → Cell Type ID → DEGs
Mass spec outputs    ──▶   LFQ → Protein quantification → Multi-omics fusion
HTS screening data   ──▶   Plate QC → Dose-response → IC50 → Hit ID
Clinical records     ──▶   Cleaning → Modeling → Statistical reports
All of the above     ──▶   Machine learning → Prediction → SHAP → Publication
```

---

## Four Roles. One Person.

<table>
<tr>
<td width="50%" valign="top">

### 🧬 Bioinformatician
Building end-to-end NGS pipelines that actually run in production. Snakemake workflows on SLURM HPC and AWS Batch. scRNA-seq with Seurat and Scanpy. Somatic variant calling with GATK Mutect2. Differential expression with DESeq2. **30% faster. 26% more throughput.** Not by accident — by design.

**Tools:** Seurat · Scanpy · DESeq2 · STAR · BWA-MEM · GATK · Mutect2 · samtools · bcftools · Snakemake · BaseSpace

</td>
<td width="50%" valign="top">

### 🤖 Data Scientist
Machine learning on biological data — where the features are genes, the labels are disease subtypes, and the stakes are real. Random Forest classifier at **AUC 0.85**. SHAP-based feature importance. 5-fold cross-validation. UMAP and PCA for dimensionality reduction. Models that generalize, not just memorize.

**Tools:** R · Python · randomForest · caret · xgboost · SHAPforxgboost · scikit-learn · pROC

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📊 Statistical Modeler
Statistics as the backbone of every analysis — not an afterthought. FDR correction on differential expression. LASSO for feature selection. Multivariate regression on clinical datasets. Proper experimental design. Cross-validation that means something. Results rigorous enough to publish and clear enough for a clinician to act on.

**Tools:** R (primary) · DESeq2 · LASSO · logistic regression · PCA · FDR · Biostatistics

</td>
<td width="50%" valign="top">

### 🗄️ Data Analyst
Raw data is almost never clean. Clinical records, formulation datasets, structured databases — every dataset has problems. SQL for querying and validation. Python scripts for integrity checks. QC protocols that catch errors before they propagate. Normalization, transformation, and reporting that R&D teams can trust.

**Tools:** SQL · Python · R · pandas · dplyr · ggplot2 · tidyr · Excel

</td>
</tr>
</table>

---

## Featured Projects

### 🔬 [scRNAseq-cancer-analysis](https://github.com/shipatel302/scRNAseq-cancer-analysis)
**Single-cell RNA-seq pipeline + Machine Learning classifier for HPV+ cancer cohorts**

A complete analysis workflow — from raw count matrices to a validated Random Forest subtype classifier. Built in R using Seurat for preprocessing, DESeq2 for differential expression, and SHAP for model interpretability.

```
QC & Filtering → Normalization → UMAP Clustering → FDR-controlled DEGs
→ Feature Matrix (top 200 DEGs + TMB scores)
→ Random Forest (5-fold CV) → AUC 0.85 → SHAP Feature Importance
```
`R` `Seurat` `DESeq2` `randomForest` `SHAP` `pROC` `ggplot2`

---

### ⚙️ [ngs-pipeline-snakemake](https://github.com/shipatel302/ngs-pipeline-snakemake)
**Production-grade NGS pipeline: somatic variant detection + transcriptomic analysis**

A Snakemake workflow covering the full NGS stack — QC, alignment, duplicate marking, base recalibration, Mutect2 variant calling, and DESeq2 differential expression. Deployable on SLURM HPC and AWS Batch. Achieves 30% runtime reduction through parallelization and optimized resource allocation.

```
FastQC → Trimmomatic → BWA-MEM → MarkDuplicates → BQSR
→ Mutect2 → FilterMutectCalls → bcftools merge
→ featureCounts → DESeq2 → MultiQC report
```
`Snakemake` `GATK4` `BWA-MEM` `Mutect2` `DESeq2` `AWS` `SLURM` `Docker`

---

### 💊 [hts-drug-screening-analysis](https://github.com/shipatel302/hts-drug-screening-analysis)
**HTS compound screening pipeline for proximity-based drug discovery (PROTACs, molecular glues)**

An R-based pipeline for processing high-throughput screening data — plate QC (Z' factor, SSMD), 4-parameter log-logistic dose-response curve fitting, IC50 estimation with 95% CI, hit identification, and downstream integration with transcriptomic and proteomic data for multi-omics candidate prioritization.

```
Plate QC (Z' factor) → 4PL Dose-Response Fitting → IC50 Estimation
→ Hit Identification → Transcriptomic + Proteomic Integration
→ Composite Prioritization Score → Ranked Candidate List
```
`R` `drc` `ggplot2` `DESeq2` `LFQ proteomics` `pheatmap`

---

## Technical Stack

```r
languages    <- c("R (primary)", "Python", "SQL", "Bash", "Linux")

omics        <- c("scRNA-seq", "Bulk RNA-seq", "WGS", "WES",
                  "Proteomics (MS/LFQ)", "Somatic Variants",
                  "TMB", "CNV", "Clinical Data", "HTS Screening")

ml_stats     <- c("Random Forest", "LASSO", "Logistic Regression",
                  "PCA", "UMAP", "SHAP", "Cross-Validation",
                  "FDR Correction", "Differential Expression",
                  "Multivariate Regression", "Dimensionality Reduction")

bio_tools    <- c("Seurat", "Scanpy", "DESeq2", "STAR", "BWA-MEM",
                  "GATK4", "Mutect2", "samtools", "bcftools",
                  "IGV", "Snakemake", "BaseSpace", "featureCounts")

infra        <- c("SLURM HPC", "AWS S3", "AWS EC2", "AWS Batch",
                  "Docker", "Git", "GitHub")
```

---

## By The Numbers

| Metric | Value |
|--------|-------|
| Years of experience | 4+ |
| Random Forest classifier AUC | 0.85 |
| Pipeline throughput improvement | +26% |
| Pipeline runtime reduction | -30% |
| Omics data types worked with | 8+ |
| Programming languages | 4 |
| GPA (M.S. Bioinformatics) | 3.8 / 4.0 |

---

## Education

🎓 **M.S. Bioinformatics Data Science** · University of Delaware · GPA 3.8 · *Expected May 2026*
*Systems Biology · Biostatistics · Machine Learning · Bioinformatics · Electronic Health Records*

🎓 **B.Pharm** · Dr. Babasaheb Ambedkar Technological University · 2022

---

## Currently Open To

```python
roles = [
    "Bioinformatics Analyst",
    "Senior Bioinformatics Analyst",
    "Computational Biologist",
    "Data Scientist (Biotech / Pharma / Healthtech)",
    "Statistical Analyst / Biostatistician",
    "Clinical Data Analyst"
]

domains = [
    "Drug Discovery",
    "Oncology",
    "Rare Disease",
    "Genomics",
    "Multi-Omics",
    "Clinical Research"
]
```

If your team works in any of these spaces — let's talk.

📧 shivanip8369@gmail.com · [LinkedIn](https://linkedin.com/in/shivanip99)

---

<div align="center">

*"Three years of working with data that does not cooperate*
*has a way of building a very specific skill set."*

</div>

