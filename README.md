# DM_ProgrammingAssignment3
Banner ID: 916539309 

This project has three parts: association analysis, CNN image classification, and BERT text classification. All work was done in Google Colab, and datasets were uploaded during runtime.

1. Association Rule Mining (Mlxtend)

Loaded the grocery transaction dataset. (Grocery_Items_9)

Found the number of unique items, total records, and the most frequent item.
Extracted association rules using support = 0.01 and confidence = 0.08.
Checked whether any 2-item antecedent rules exist (none did).
Created a heatmap showing how different support/confidence values affect the number of rules.

Key observation:
Lower thresholds produce many rules; higher thresholds produce fewer, stronger rules.

2. CNN Image Classification

Dataset: (New_Dataset_CNN)
Used my 4-class image dataset (buildings, forest, glacier, sea).

Built the CNN with the required architecture: two Conv2D layers, pooling, flatten, Dense(8), and a softmax output.

Trained for 20 epochs with 20% validation split.
Plotted training/validation accuracy curves.

Experiment (Banner ID ends in 9 → option C):
Changed the hidden layer to 4 nodes and 16 nodes and plotted their learning curves.

Finding:
4 nodes → underfits a bit.
16 nodes → learns faster but may overfit.
Base model stays balanced.

3. BERT Text Classification (Multi-label)

Dataset: (Text Data- 9)
Used the tweet emotion dataset (11 labels).

Tokenized using BERT-base-uncased.
Fine-tuned the model for 5 epochs.
Plotted training and validation losses.

Test accuracy:

Exact match accuracy: 0.25
At least one label correct: 0.862
The second method gives a clearer view of how well the model captures emotional cues.
