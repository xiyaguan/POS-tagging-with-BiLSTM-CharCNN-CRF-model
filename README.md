# POS-tagging-with-BiLSTM-CharCNN-CRF-model
Task definition: POS tagging is the task of assigning a POS tag to each word token in the sentence, and it is a typical sequence labeling problem. 

Note: In this project, you will get to know how to implement a charCNN layer and CRF layer from scratch.

The agenda of this implementation
1. Processed data samples using two pytorch data primitives: Dataset & dataloader
2. Replaced the randomly initialized embeddings with pre-trained word embeddings: GloVe
3. Built up LSTM-CNNs-CRF model, this includes 3 layers: 
   A. charCNN layer where CharCNNEmbeddings - a self-defined charCNN encoder for char level embeddings, will be called to output char embeddings;  
   B. biLSTM layer; 
   C. CRF layer;
5. Training & validating on each epoch
6. Tested on dataset and saved output to two files in “output” folder: “output/output.tag” and “output/output.tagged”, with the same order of sequences as the test dataset file “test/ptb_23.snt”. 
