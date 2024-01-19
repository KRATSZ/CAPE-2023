# CAPE-2023
Official Repository for Critical Assessment of Protein Engineering(CAPE)

<a href="https://www.kaggle.com/code/mecoywittergreen/siat-baseline"><img src="https://img.shields.io/badge/Kaggle-Notebook-%2355555)"></a> 
<a href="https://colab.research.google.com/drive/1_1LzDzTNxX-6KVUwoJTi0sMHs4CFJ2NR#scrollTo=x2gWDnaDtsN2"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> </a>

*Note*: CAPE was held during October 2023 as a data challenge and workshop. This README and the related links provide an overview of the competition and archive the artifacts from the event to serve the CAPE community. 
*Important*: This README is an archive for the event and the workshop, all the code, data, tests and code are available. 
## Overview
The goal of this competition is to predict how mutations in specific amino acids affect enzyme function, focusing on RhlA, a key enzyme in producing rhamnolipids—a promising biosurfactant with applications across various industries. Rhamnolipids are hindered by high production and separation costs due to their structural homologues.Enhancing RhlA's selectivity could streamline production and reduce costs. 

<div align="center">
    <img src="https://github.com/KRATSZ/CAPE-2023/assets/59955777/74e902e6-a3e5-47a4-b694-4aa489de18d2" alt="描述文字" width="500"/>
</div>

However, Current experimental methods are slow, but **automated synthetic biology** can rapidly test mutations.It can quickly achieve specific functions through low-cost, multi-cycle large-scale engineering trial and error experiments. Based on a robotic platform facility, the automated construction and testing of RhlA's unit point saturation mutations and multi-site combinatorial mutation libraries have been realized.

### Quick links

* 📖 [Kaggle competition website](https://www.kaggle.com/competitions/siatprotein2023)
* 📖 [The solution from different team](https://www.kaggle.com/competitions/siatprotein2023/code)
* 📖 [Some of our previous work and the origin of part of the dataset](https://academic.oup.com/bib/article/24/1/bbac570/6958505)

## Dataset
### Introduction to "training.csv" (Training Dataset)

This is the training data for the competition, in CSV format, containing a total of 1593 sequences.
The first column is called "Sequence," corresponding to combinations of different mutation sites. A combination of six letters represents the mutations at six sites, which are the amino acids at positions 74, 101, 143, 148, 173, and 176. These positions have been identified as the most effective mutation sites in our actual tests.
The last two columns are enzyme function evaluation indicators, including (1) Normalized Activity: the total yield of enzyme catalytic activity for Rhla-C20 and Rhla-C18. (2) Normalized Selectivity: the selectivity of the enzyme, which is the ratio of Rhla-C18 to the total yield.
![image](https://github.com/KRATSZ/CAPE-2023/assets/59955777/c0403a4f-2452-4d3b-be98-cd53a36de529)

### Introduction to "test.csv" (Test Dataset)

Here are 925 new pieces of data. They contain sequence information but do not include corresponding activity and selectivity. The participant need to predict the activity and selectivity associated with these sequences and obtain feedback to know the overall predictive capability of participant's model.

Prediction and Feedback: To fully understand the performance of the model, participants need to use their algorithms to predict the enzyme activity and selectivity corresponding to the sequences in "test.csv." At the same time, participants can submit their predictions for "test.csv" on Kaggle to receive feedback on their models.

![image](https://github.com/KRATSZ/CAPE-2023/assets/59955777/8c20be3b-fb45-4b4f-b3ac-045391f2fe54)


## Useful resources
💯 Although we have provided a sequence training set and test set, participants can also **use many other resources** for training to improve the final results. We believe the following resources are of high quality, and may consider using them to enhance the effectiveness of the model:

1. *UniProtKB*: This is a primary resource for protein function annotation. It contains sequences and many links to other databases.
2. *Gene Ontology (GO)*: This database is for enzyme function ontology. It also contains some annotations of protein-gene functions.
3. *Protein Data Bank (PDB)*: A database of protein structures.
4. *STRING*: A website for studying protein interactions.
5. *GEO*: A database website for gene expression data.
6. *PRIDE*: A database of proteins identified through mass spectrometry experiments.

The page at https://en.wikipedia.org/wiki/Rhamnolipid provides detailed information about rhamnolipids, including their chemical structure and biosynthetic pathways.

The article at https://www.pnas.org/doi/10.1073/pnas.2101366118 mentions that HAAs (3-hydroxyacyl-ACP) are synthesized in Pseudomonas aeruginosa by the enzyme RhlA through the dimerization of (R)-3-hydroxyacyl-CoA.

The article at https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7054101/ discusses the diversity of the RhlA enzyme and how this diversity can be exploited to synthesize different rhamnolipids.
