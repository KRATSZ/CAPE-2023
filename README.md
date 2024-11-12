# CAPE
WELCOME!Here is official Repository for Critical Assessment of Protein Engineering(CAPE)

<a href="https://www.kaggle.com/code/mecoywittergreen/siat-baseline"><img src="https://img.shields.io/badge/Kaggle-Notebook-%2355555)"></a> 
<a href="https://colab.research.google.com/drive/1_1LzDzTNxX-6KVUwoJTi0sMHs4CFJ2NR#scrollTo=x2gWDnaDtsN2"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> </a>


*Note*: CAPE was held during October 2023 as a data challenge and workshop. This README and the related links provide an overview of the competition and archive the artifacts from the event to serve the CAPE community. 
We have partnered with SAPROT to enable undergraduate students to build models and predict sequences using CAPE's dataset with just a few clicks：
<a href="https://colab.research.google.com/drive/1RFfdVtrPM0PKQHMoiSqlCoXvns6QmgKD#scrollTo=urgvFgkIjKtT"> <img src="https://colab.research.google.com/assets/colab-badge.svg"> </a>
*Important*: This README is an archive for the event and the workshop, all the code, data, tests and code are available. 

## Overview
The goal of this competition is to predict how mutations in specific amino acids affect enzyme function, focusing on RhlA, a key enzyme in producing rhamnolipids—a promising biosurfactant with applications across various industries. Rhamnolipids are hindered by high production and separation costs due to their structural homologues.Enhancing RhlA's selectivity could streamline production and reduce costs. 

<div align="center">
    <img src="https://github.com/KRATSZ/CAPE-2023/assets/59955777/74e902e6-a3e5-47a4-b694-4aa489de18d2" alt="描述文字" width="500"/>
</div>

However, Current experimental methods are slow, but **automated synthetic biology** can rapidly test mutations.It can quickly achieve specific functions through low-cost, multi-cycle large-scale engineering trial and error experiments. Based on a robotic platform facility, the automated construction and testing of RhlA's unit point saturation mutations and multi-site combinatorial mutation libraries have been realized.
### The Round1 
Round 1 was organized as synbio Challenges, as part of the synbio Challenges competition, players constructed and predicted 96 optimal sequences for mutations to submit. Players were invited to give offline PPT presentations and algorithm explanations, and the team with the best results was finally evaluated.

### The Round2
The Protein Design PLUS Competition, hosted on the Shenzhen Synthetic Biology Research Infrastructure's cloud platform and Kaggle, aims to foster cross-disciplinary student engagement in AI-driven protein design. Building on the inaugural SC Protein Design Competition, it continues to concentrate on machine learning for enzyme engineering, targeting the eco-friendly production of biosurfactants. 

Contestants accessed a dataset of the enzyme RhlA on Kaggle, refining their predictive models through feedback from a hidden validation set. Teams then designed sequences that were tested at the Big Facility, with rankings based on experimental outcomes.

![image (1)](https://github.com/KRATSZ/CAPE-2023/assets/59955777/644be513-c701-4f59-a657-2645d457985a)

### Goal
We provide information about protein structure and function, including all amino acid sequences, 6 candidate mutation sites, target performance and performance measurements to be optimized, and thousands of sequence-performance data. Contestants *selected 96 mutation sequences* from the mutation design space of 20^6 and submitted them to the competition, and all the participating sequences were constructed and measured by the Synthetic Biology Facility 

### Quick links

* 📖 [Kaggle competition website](https://www.kaggle.com/competitions/siatprotein2023)
* 📖 [The solution from different team](https://www.kaggle.com/competitions/siatprotein2023/code)
* 📖 [Some of our previous work and the origin of part of the dataset](https://academic.oup.com/bib/article/24/1/bbac570/6958505)

## Dataset
### "training.csv" (Training Dataset)

This is the training data for the competition, in CSV format, containing a total of 1593 sequences.
The first column is called "Sequence," corresponding to combinations of different mutation sites. A combination of six letters represents the mutations at six sites, which are the amino acids at positions 74, 101, 143, 148, 173, and 176. These positions have been identified as the most effective mutation sites in our actual tests.
The last two columns are enzyme function evaluation indicators, including (1) Normalized Activity: the total yield of enzyme catalytic activity for Rhla-C20 and Rhla-C18. (2) Normalized Selectivity: the selectivity of the enzyme, which is the ratio of Rhla-C18 to the total yield.
![image](https://github.com/KRATSZ/CAPE-2023/assets/59955777/a5c58263-7287-43ca-a98f-fb6aa8bdd34f)


### "test.csv" (Test Dataset)

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

## Organizers
This Data Challenge was built in the open, with the goal of adding lasting artifacts to the community. CAPE hope be a collaboration between industry and academia, who joined forces to make it happen:

* [Shenzhen Institute of Advanced Technology(SIAT)](https://www.siat.ac.cn/)，Chinese Academy of Sciences
* [Shenzhen Institute of Synthetic Biology large facility](https://www.linkedin.com/in/gabrielspmoreira/), SIAT
* [Sitong](https://isynbio.siat.ac.cn/sitonglab/), SIAT
* [Yixiao](http://www.isynbio.org/team-detail.aspx?detail=2610&parm=1671), SIAT
![image](https://github.com/KRATSZ/CAPE-2023/assets/59955777/9db360ee-2e27-4913-9039-dc71636f266d)

