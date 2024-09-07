**Track 3: Data Science and Machine Learning**

**Research Paper Title:** _‘Large-scale RNA-Seq Transcriptome Analysis of 4043 Cancers and 548 Normal Tissue Controls across 12 TCGA Cancer Types’_

**Paper Link :** <https://www.nature.com/articles/srep13413> 

**Authors:** Mahima Chakraborty (@mahima\_ch), Tamosree Das (@Tamosree), Obianujunwa Martha Ugota (@obianujunwa), Faheem Ahmed Khan (@Faheem.Za) 

**GitHub Link:** <https://github.com/mahiiC/HackBio_Internship_2024/blob/main/Stage_1_task.md>

**Introduction** 

Changes in gene expression patterns caused by build-up of mutations or epigenetic alterations are regarded to be the primary source of cancer. In comparison to microarrays, RNA-Seq is a novel method that provides genome-wide gene expression profiling and has numerous benefits, including a superior ability to define the transcriptome alterations linked to human malignancies. With the help of records from the TCGA data portal, this study compared and analyzed the RNA-Seq transcriptomes of 4043 cancer and 548 solid tissue normal samples across 12 types of cancer using the edgeR Bioconductor package, differential expression analysis of individual genes, clustering and gene set association analysis, pathway enrichment analysis and disease association analysis to enable a biological understanding of the genes and how they play a role in cancer development.

**Methods** 

Transcriptome and clinical data from TCGA were used, with an emphasis on the UNC platform (IlluminaHiSeq\_RNASeqV2) to reduce sequencing variability. Twelve cancer types were chosen, having data from both malignant and normal tissues. EdgeR was used to do differential expression analysis between "primary tumor" and "solid tissue normal" samples.  Genes were grouped into co-regulated sets utilizing DESeq normalization and APCluster, and expression similarity was measured using Pearson correlation. GSAASeqSP was used to assess gene set association, screening out gene sets with fewer than 15 or more than 100 genes and applying an FDR limit of 0.15. WebGestalt was used to conduct pathway and disease association analyses, which included GO, KEGG, and Pathway Commons analysis.

**Results** 

Gene-level differential expression analysis of transcriptomes showed the percentage of common genes differentially expressed (DE) in different cancer types, e.g. LUAD and LUSC showed a 55% similarity in DE genes, whereas KICH and KIRC showed below 10% similarity. Clustering and gene-set association analysis of the clusters identified seven cross-cancer gene signatures regulating the cell cycle altered across four cancer types. Cancer-specific gene signatures were also identified for lung cancer, BLCA, BRCA, and KICH.

A 14-gene signature was created by selecting the top two DE genes from the seven gene sets identified earlier. This was used to accurately classify normal and cancerous tissue samples by Leave-one-out cross-validation (LOOCV) using SVM-light, an ML technique. The results were further validated using non-TCGA datasets.

**Discussion & Conclusion**

This research offers a comprehensive gene expression analysis of 4043 cancer samples and 548 normal tissue samples across 12 cancer types, revealing crucial gene signatures common to multiple cancers and specific to individual cancer types. The results highlight the central importance of cell cycle control in cancer development and provide valuable knowledge about the molecular pathways involved in tumor formation. By identifying potential biomarkers for diagnosis and targets for therapy, the study demonstrates the significance of large-scale RNA sequencing data in enhancing cancer research and potentially improving patient outcomes.

**Reference**

Peng, L., Bian, X. W., Li, D. K., Xu, C., Wang, G. M., Xia, Q. Y., & Xiong, Q. (2015). Large-scale RNA-Seq Transcriptome Analysis of 4043 Cancers and 548 Normal Tissue Controls across 12 TCGA Cancer Types. Scientific Reports, 5(1), 1-18. <https://doi.org/10.1038/srep13413> 

