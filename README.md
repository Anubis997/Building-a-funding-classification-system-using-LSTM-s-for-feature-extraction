# Donors-Choose-dataset-using-Deep-Learning
1. Split the data into test size of 0.3. Tokenized text corpus and Synthesized an embedding matrix using pretrained_glove vectors. 
2. Constructed 2 different architectures using Keras functional Api's, using LSTM for essay corpus and trainable embedding layers.
3. Developed custom callback functions for earlystopping, learningrate scheduling and test metrics such as AUC, F1-score and recall.
4. Boosted AUC to 0.91 from an AUC of 0.73 by using single layer of embedding for text and numerical data and LSTM's on essay corpus.
   Extrapolated weights and scores using Tensorboard graphs.
