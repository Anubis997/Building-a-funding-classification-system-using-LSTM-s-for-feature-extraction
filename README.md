# Donors-Choose-dataset-using-Deep-Learning
Data Preprocessing: The total text data columns are used as input. The GloVe word vectors are employed via an embedding layer, without training the word vectors. Several categorical columns such as 'school_state', 'project_grade_category', 'input_clean_categories', 'input_clean_subcategories', and 'input_teacher_prefix' are also used as inputs to separate embedding layers.

LSTM and Flatten: The LSTM layer is applied to the text data embedded by the embedding layer, resulting in an LSTM output. The LSTM output is then flattened.

Dense Layers: The remaining columns are concatenated, and a dense layer is added. The concatenated output from the dense layer is further passed through a series of dense layers, followed by batch normalization.

Model Architecture: The flattened LSTM output, flattened embedding layers, dense layer output, and the remaining columns are concatenated. This concatenated tensor is then passed through additional dense and batch normalization layers.

Model Training: The model is trained using the given architecture and the AUC metric. Three types of models are trained, but specific details about the other models are not provided in the given information.

Optimization: An optimizer is used during training, along with a specified learning rate and momentum.

TensorBoard and Visualization: TensorBoard is utilized to monitor the training progress. Metrics such as loss and accuracy are plotted over epochs.

Succesfully built a classification system with 0.75 val_auc.
