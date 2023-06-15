# TCR-HLA-peptide binding

## Intros

**T-cell receptor (TCR), peptide, and human leukocyte antigen (HLA) interactions** play a crucial role in the adaptive immune response, orchestrating the recognition and targeting of foreign substances, such as pathogens or cancer cells. **TCRs are specialized proteins found on the surface of T lymphocytes**, which are a type of white blood cell responsible for immune surveillance and response. These receptors have the remarkable ability to **recognize specific peptide antigens presented by HLA molecules, also known as major histocompatibility complex (MHC) molecules, on the surface of antigen-presenting cells.**

Peptides are short chains of amino acids, the building blocks of proteins, and are derived from various sources, including proteins from pathogens or self-proteins altered by disease processes. The generation of peptide antigens is a complex process involving the degradation of proteins within the cell, followed by their presentation on the cell surface through the binding with HLA molecules. **HLA molecules are highly polymorphic proteins that act as molecular platforms, presenting a diverse range of peptides to TCRs.** This interaction serves as a critical determinant for the activation and regulation of T-cell responses.

**The binding of TCRs to specific peptide-HLA complexes triggers a cascade of signaling events within T cells, leading to their activation and subsequent immune responses.** This recognition mechanism enables the immune system to detect and respond to a vast array of potential threats.

Understanding the TCR-peptide-HLA interaction has significant implications in immunology, infectious diseases, autoimmune disorders, and cancer immunotherapy. It provides insights into the development of vaccines, immunomodulatory therapies, and personalized medicine approaches. Moreover, studying the diversity and dynamics of TCR-peptide-HLA interactions contributes to our understanding of immune evasion mechanisms employed by pathogens and tumors, guiding the design of strategies to overcome these evasive tactics.

## Biological domain knowledge
|HLA-pep binding|TCR-HLA-pep binding|
|:-:|:-:|
|<img src="imgs/hla-pep.jpg">|<img src="imgs/tcr-hla-pep.png">|
<!-- |[Image source](https://microbiologynotes.org/major-histocompatibility-complex-mhc-introduction-types-and-differences/)|[Image source](https://www.researchgate.net/figure/MHC-class-I-and-class-II-and-their-role-as-mediators-during-antigen-presentation-and_fig1_280663544)| -->
- [ ] **[Structure of the complex between human T-cell receptor, viral peptide and HLA-A2](http://www.nature.com/articles/384134a0) (1996 Nature)**
  - "The interface between TCR and MHC/pcptide is in unambiguous electron density, as are 
  - the $\alpha$ 1, $\alpha$ 2, and $\beta$ 2-microglobulin ($\beta$ 2m) domains of the MHC 
  - and the V $\alpha$ and V $\beta$ domains of the TCR."
- [ ] **[Classification of Human Leukocyte Antigen (HLA) Supertypes](http://link.springer.com/10.1007/978-1-4939-1115-8_17) (2014 Immunoinformatics)**
- [ ] **[Predicting Antigen Presentationwhat Could we Learn From a Million Peptides?](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6068240/)**

## HLA-Peptide Interaction

### Surveys

- [ ] **[Toward more accurate pan-specific MHC-peptide binding prediction: a review of current methods and tools](https://pubmed.ncbi.nlm.nih.gov/21949215/)**

This paper is a review of current methods and tools for predicting the binding of short antigenic peptides to major histocompatibility complex (MHC) molecules. The precise identification of MHC-restricted peptides is important for understanding the mechanism of immune response and discovering immunogenic epitopes. However, due to the high polymorphism of MHC molecules and the cost of biochemical experiments, computational approaches have become increasingly important for predicting peptide binding. Pan-specific methods, which use experimentally obtained binding data of multiple alleles, have received keen interest in recent years. This article extensively reviews existing pan-specific methods and their web servers, presenting a general framework for these methods. Additionally, we provide a brief overview of comparative studies on the performance of different prediction methods using several independent data sets.

### Traditional methods
Pseudo sequence is always used to represent HLA in Pan-specific methods.
- [ ] **[NetMHCpan, a Method for Quantitative Predictions of Peptide Binding to Any HLA-A and -B Locus Protein of Known Sequence](https://dx.plos.org/10.1371/journal.pone.0000796) (2007)**
- [ ] **[NetMHCpan-4.0: Improved Peptide–MHC Class I Interaction Predictions Integrating Eluted Ligand and Peptide Binding Affinity Data](https://journals.aai.org/jimmunol/article/199/9/3360/109797/NetMHCpan-4-0-Improved-Peptide-MHC-Class-I) (2017)**
- [ ] **[[TransPHLA] A transformer-based model to predict peptide–HLA class I binding and optimize mutated peptides for vaccine design](https://www.nature.com/articles/s42256-022-00459-7) (2022 NMI)**

### Pre-trained language model-based methods

- [ ] **[Interpreting BERT architecture predictions for peptide presentation by MHC class I proteins](https://arxiv.org/abs/2111.07137)**

- [ ] **[Improved Predictions of MHC-Peptide Binding using Protein Language Models](https://www.biorxiv.org/content/10.1101/2022.02.11.479844v1)**

## TCR-HLA-peptide interaction

Although a TCR binds to an epitope and the corresponding MHC molecule partner simultaneously, the core binding regions of the complex are between the **complementarity determining region 3 of the TCR β chain (CDR3β) and the epitope**

- [ ] **[Current challenges for unseen-epitope TCR interaction prediction and a new perspective derived from image classification](https://academic.oup.com/bib/article/22/4/bbaa318/6042663)**
  - **Unseen epitope**

- [ ] **[Contribution of T Cell Receptor Alpha and Beta CDR3, MHC Typing, V and J Genes to Peptide Binding Prediction](https://www.frontiersin.org/articles/10.3389/fimmu.2021.664514/full)**

- [ ] **[[pMTnet] Deep learning-based prediction of the T cell receptor–antigen binding specificity](https://www.nature.com/articles/s42256-021-00383-2)**
  - The online tool is available at https://dbai.biohpc.swmed.edu/pmtnet/index.php
    - (**Highlights**) The **subsequent** pMTnet version 

- [ ] **[Detection of Enriched T Cell Epitope Specificity in Full T Cell Receptor Sequence Repertoires](https://www.frontiersin.org/articles/10.3389/fimmu.2019.02820/full)**
- [ ] **[Pan-Peptide Meta Learning for T-cell receptor–antigen binding recognition](https://www.nature.com/articles/s42256-023-00619-3)**
- [ ] **[Characterizing the interaction conformation between T-cell receptors and epitopes with deep learning](https://www.nature.com/articles/s42256-023-00634-4)**


## Protein language models
- [ ] **[[Survey] Learning functional properties of proteins with language models](https://www.nature.com/articles/s42256-022-00457-9) (2022 NMI)**
  - sequence-based
- [ ] **[[Survey] A Survey on Protein Representation Learning: Retrospect and Prospect](http://arxiv.org/abs/2301.00813) (2023 arxiv)**
  - sequence-based, structure-based, and sequence-structure co-modeling
  - Methods mentioned in the paper are summarized in their [Reading List](https://github.com/LirongWu/awesome-protein-representation-learning).
- [ ] **[[Survey] PEER: A Comprehensive and Multi-Task Benchmark for Protein Sequence Understanding](https://arxiv.org/abs/2206.02096)**

---
<img src="imgs/protein-structure_cut.png" title="Protein structure level" width=80%>

## Towards structure-based methods

- [ ] **[[AlphaFold2] Highly accurate protein structure prediction with AlphaFold](https://www.nature.com/articles/s41586-021-03819-2)**
- [ ] **[[ESMFold] Evolutionary-scale prediction of atomic-level protein structure with a language model](https://www.science.org/doi/10.1126/science.ade2574)**
- [ ] **[[Survey] Protein Language Models and Structure Prediction: Connection and Progression](https://arxiv.org/abs/2211.16742)**

Fine-tune AlphaFold2 (Philip Bradley & David Baker):
- [ ] **[Structure-based prediction of T cell receptor: peptide-MHC interactions](https://elifesciences.org/articles/82813)**
- [ ] **[Peptide-binding specificity prediction using fine-tuned protein structure prediction networks](https://www.pnas.org/doi/10.1073/pnas.2216697120)**

## General protein-ligand interaction

### Sequence-based

### Structure-based

