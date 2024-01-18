## Dataset
### Introduction to "training.csv" (Training Dataset)

This is the training data for the competition, in CSV format, containing a total of 1593 sequences.
The first column is called "Sequence," corresponding to combinations of different mutation sites. A combination of six letters represents the mutations at six sites, which are the amino acids at positions 74, 101, 143, 148, 173, and 176. These positions have been identified as the most effective mutation sites in our actual tests.
The last two columns are enzyme function evaluation indicators, including (1) Normalized Activity: the total yield of enzyme catalytic activity for Rhla-C20 and Rhla-C18. (2) Normalized Selectivity: the selectivity of the enzyme, which is the ratio of Rhla-C18 to the total yield.
![image](https://github.com/KRATSZ/CAPE-2023/assets/59955777/c0403a4f-2452-4d3b-be98-cd53a36de529)

### Introduction to "test.csv" (Test Dataset)

Here are 925 new pieces of data. They contain sequence information but do not include corresponding activity and selectivity. The participant need to predict the activity and selectivity associated with these sequences and obtain feedback to know the overall predictive capability of participant's model.

Prediction and Feedback: To fully understand the performance of the model, participants need to use their algorithms to predict the enzyme activity and selectivity corresponding to the sequences in "test.csv." At the same time, participants can submit their predictions for "test.csv" on Kaggle to receive feedback on their models.

