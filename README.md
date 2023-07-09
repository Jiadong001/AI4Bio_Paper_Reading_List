# Protein domain
<img src="https://img.shields.io/badge/Protein-TCR_HLA_peptide-red.svg?logo=LOGO">
<img src="https://img.shields.io/badge/Protein-Sequence_Design-red.svg?logo=LOGO">
<img src="https://img.shields.io/badge/Protein-Structure_Prediction-red.svg?logo=LOGO">
<img src="https://img.shields.io/badge/AI-Language_Model-green.svg?logo=LOGO">
<img src="https://img.shields.io/badge/AI-AlphaFold-green.svg?logo=LOGO">


## 1. TCR-HLA-peptide Binding Prediction

### Intros

**T-cell receptor (TCR), peptide, and human leukocyte antigen (HLA) interactions** play a crucial role in the adaptive immune response, orchestrating the recognition and targeting of foreign substances, such as pathogens or cancer cells. 

<details>
  <summary>More details</summary>

  **TCRs are specialized proteins found on the surface of T lymphocytes**, which are a type of white blood cell responsible for immune surveillance and response. These receptors have the remarkable ability to **recognize specific peptide antigens presented by HLA molecules, also known as major histocompatibility complex (MHC) molecules, on the surface of antigen-presenting cells.**

  Peptides are short chains of amino acids, the building blocks of proteins, and are derived from various sources, including proteins from pathogens or self-proteins altered by disease processes. The generation of peptide antigens is a complex process involving the degradation of proteins within the cell, followed by their presentation on the cell surface through the binding with HLA molecules. **HLA molecules are highly polymorphic proteins that act as molecular platforms, presenting a diverse range of peptides to TCRs.** This interaction serves as a critical determinant for the activation and regulation of T-cell responses.

  **The binding of TCRs to specific peptide-HLA complexes triggers a cascade of signaling events within T cells, leading to their activation and subsequent immune responses.** This recognition mechanism enables the immune system to detect and respond to a vast array of potential threats.

  Understanding the TCR-peptide-HLA interaction has significant implications in immunology, infectious diseases, autoimmune disorders, and cancer immunotherapy. It provides insights into the development of vaccines, immunomodulatory therapies, and personalized medicine approaches. Moreover, studying the diversity and dynamics of TCR-peptide-HLA interactions contributes to our understanding of immune evasion mechanisms employed by pathogens and tumors, guiding the design of strategies to overcome these evasive tactics.

</details>


### Biological domain knowledge
|HLA-pep binding|TCR-HLA-pep binding|
|:-:|:-:|
|<img src="imgs/hla-pep.jpg">|<img src="imgs/tcr-hla-pep.png">|

- [ ] **[Structure of the complex between human T-cell receptor, viral peptide and HLA-A2](http://www.nature.com/articles/384134a0) (1996 Nature)**

  <details>
    <summary>Note</summary>

  >"The interface between TCR and MHC/pcptide is in unambiguous electron density, as are the α1, α2, and β2-microglobulin (β2m) domains of the MHC and the Vα and Vβ domains of the TCR."

  </details>

- [ ] **[Classification of Human Leukocyte Antigen (HLA) Supertypes](http://link.springer.com/10.1007/978-1-4939-1115-8_17) (2014 Immunoinformatics)**
- [ ] **[Predicting Antigen Presentationwhat Could we Learn From a Million Peptides?](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6068240/)**


### HLA-Peptide interaction

#### Surveys

- [ ] **[Toward more accurate pan-specific MHC-peptide binding prediction: a review of current methods and tools](https://pubmed.ncbi.nlm.nih.gov/21949215/)**

  <details>
    <summary>Note</summary>

    This paper is a review of current methods and tools for predicting the binding of short antigenic peptides to major histocompatibility complex (MHC) molecules. The precise identification of MHC-restricted peptides is important for understanding the mechanism of immune response and discovering immunogenic epitopes. However, due to the high polymorphism of MHC molecules and the cost of biochemical experiments, computational approaches have become increasingly important for predicting peptide binding. **Pan-specific methods**, which use experimentally obtained binding data of multiple alleles, have received keen interest in recent years. This article extensively reviews existing pan-specific methods and their web servers, presenting a general framework for these methods. Additionally, we provide a brief overview of comparative studies on the performance of different prediction methods using several independent data sets.

    </details>


#### Traditional methods
Pseudo sequence is always used to represent HLA in Pan-specific methods.
- [ ] **[NetMHCpan, a Method for Quantitative Predictions of Peptide Binding to Any HLA-A and -B Locus Protein of Known Sequence](https://dx.plos.org/10.1371/journal.pone.0000796) (2007)**
- [ ] **[NetMHCpan-4.0: Improved Peptide–MHC Class I Interaction Predictions Integrating Eluted Ligand and Peptide Binding Affinity Data](https://journals.aai.org/jimmunol/article/199/9/3360/109797/NetMHCpan-4-0-Improved-Peptide-MHC-Class-I) (2017)**
- [ ] **[[TransPHLA] A transformer-based model to predict peptide–HLA class I binding and optimize mutated peptides for vaccine design](https://www.nature.com/articles/s42256-022-00459-7) (2022 NMI)**
- [ ] **[HLAncPred: a method for predicting promiscuous non-classical HLA binding sites](https://academic.oup.com/bib/article-abstract/23/5/bbac192/6587168?redirectedFrom=fulltext) (2022 Bioinformatics)**


#### Pre-trained language model-based methods

- [ ] **[Interpreting BERT architecture predictions for peptide presentation by MHC class I proteins](https://arxiv.org/abs/2111.07137)**

- [ ] **[Improved Predictions of MHC-Peptide Binding using Protein Language Models](https://www.biorxiv.org/content/10.1101/2022.02.11.479844v1)**


### TCR-HLA-peptide interaction

Although a TCR binds to an epitope and the corresponding MHC molecule partner simultaneously, the core binding regions of the complex are between the **complementarity determining region 3 of the TCR β chain (CDR3β) and the epitope**.

- [ ] **[Current challenges for unseen-epitope TCR interaction prediction and a new perspective derived from image classification](https://academic.oup.com/bib/article/22/4/bbaa318/6042663)**
  - **Unseen epitope**

- [ ] **[Contribution of T Cell Receptor Alpha and Beta CDR3, MHC Typing, V and J Genes to Peptide Binding Prediction](https://www.frontiersin.org/articles/10.3389/fimmu.2021.664514/full)**

- [ ] **[[pMTnet] Deep learning-based prediction of the T cell receptor–antigen binding specificity](https://www.nature.com/articles/s42256-021-00383-2)**
  - The online tool is available at https://dbai.biohpc.swmed.edu/pmtnet/index.php
    - (**Highlights**) The **subsequent** pMTnet version 

- [ ] **[Detection of Enriched T Cell Epitope Specificity in Full T Cell Receptor Sequence Repertoires](https://www.frontiersin.org/articles/10.3389/fimmu.2019.02820/full)**
- [ ] **[Pan-Peptide Meta Learning for T-cell receptor–antigen binding recognition](https://www.nature.com/articles/s42256-023-00619-3)**
- [ ] **[Characterizing the interaction conformation between T-cell receptors and epitopes with deep learning](https://www.nature.com/articles/s42256-023-00634-4)**
- [ ] **[DeepTCR is a deep learning framework for revealing sequence concepts within T-cell repertoires](https://www.nature.com/articles/s42256-023-00634-4)**
  - Follow-up work: **[Deep learning reveals predictive sequence concepts within immune repertoires to immunotherapy](https://www.science.org/doi/10.1126/sciadv.abq5089)**

Potential data resources:
- [ ] **[Facile repurposing of peptide–MHC-restricted antibodies for cancer immunotherapy](https://www.nature.com/articles/s41587-022-01567-w) (2023 NBT)**

### Towards structure-based methods
Fine-tune AlphaFold2 (Philip Bradley & David Baker):
- [ ] **[Peptide-binding specificity prediction using fine-tuned protein structure prediction networks](https://www.pnas.org/doi/10.1073/pnas.2216697120) (2023)**
- [ ] **[Structure-based prediction of T cell receptor: peptide-MHC interactions](https://elifesciences.org/articles/82813) (2023)**


## 2. Protein (Pre-trained) Language Models

Amino acid sequence -- protein language

### Surveys
- [ ] **[Learning functional properties of proteins with language models](https://www.nature.com/articles/s42256-022-00457-9) (2022 NMI)**
  - sequence-based
- [ ] **[PEER: A Comprehensive and Multi-Task Benchmark for Protein Sequence Understanding](https://arxiv.org/abs/2206.02096) (2022 NIPS)**
- [ ] **[A Survey on Protein Representation Learning: Retrospect and Prospect](http://arxiv.org/abs/2301.00813) (2023 arxiv)**
  - sequence-based, structure-based, and sequence-structure co-modeling
  - Methods mentioned in the paper are summarized in their [awesome-protein-representation-learning](https://github.com/LirongWu/awesome-protein-representation-learning).


### Representative models

BERT-based:
- [ ] **[Evaluating Protein Transfer Learning with TAPE](http://biorxiv.org/lookup/doi/10.1101/676825) (2019 NIPS)**
- [ ] **[[ESM-1b] Biological structure and function emerge from scaling unsupervised learning to 250 million protein sequences](https://www.pnas.org/doi/full/10.1073/pnas.2016239118) (2020 PNAS)**
- [ ] **[MSA Transformer](https://www.biorxiv.org/content/10.1101/2021.02.12.430858v1) (2021 bioRxiv)**
  - https://zhuanlan.zhihu.com/p/359280937


GLM-based:
- [ ] **[xTrimoPGLM: Unified 100B-Scale Pre-trained Transformer for Deciphering the Language of Protein](https://www.biorxiv.org/content/10.1101/2023.07.05.547496v1) (2023 | Baidu BioMap)**


### Applications
- [ ] **[Efficient evolution of human antibodies from general protein language models](https://www.nature.com/articles/s41587-023-01763-2) (2023 NBT)**


## 3. Structure Prediction

<img src="imgs/protein-structure_cut.png" title="Protein structure level" width=80%>

### Surveys
- [ ] **[Protein Language Models and Structure Prediction: Connection and Progression](https://arxiv.org/abs/2211.16742)**


### State-of-the-art methods
- [ ] **[[AlphaFold2] Highly accurate protein structure prediction with AlphaFold](https://www.nature.com/articles/s41586-021-03819-2) (2021 Nature)**
- [ ] **[[ESMFold] Evolutionary-scale prediction of atomic-level protein structure with a language model](https://www.science.org/doi/10.1126/science.ade2574) (2023 Science)**


## 4. Sequence Design

- [ ] **[Robust deep learning–based protein sequence design using ProteinMPNN](http://biorxiv.org/lookup/doi/10.1101/2023.02.03.526917)**
- [ ] **[[LM-Design] Structure-informed Language Models Are Protein Designers](http://biorxiv.org/lookup/doi/10.1101/2023.02.03.526917)**


https://mp.weixin.qq.com/s/KfAdtdo9Rs4PP-DHlCO7aA


## 5. General protein-ligand interaction

### Sequence-based
- [ ] **[MGPLI: exploring multigranular representations for protein–ligand interaction prediction](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btac597/6696233) (2022 Bioinformatics)**


### Structure-based


---
# Other domains
- [ ] **[[Geneformer] Transfer learning enables predictions in network biology](https://www.nature.com/articles/s41586-023-06139-9) (2023 Nature)**
- [ ] **[CancerGPT: Few-shot Drug Pair Synergy Prediction using Large Pre-trained Language Models](http://arxiv.org/abs/2304.10946) (2023 arxiv)**