# Key-Point-Analysis/TouristReviews
This repository contains the code for Fine-tuning the BERT model to calculate the similarity score between two sentences. The Argument and Key-pointwere given as the input along with special tokens [CLS] at the beginning and the [SEP] token between Argument and
Key-point. Trained the model for 3 epochs by adding a linear fully connected layer of size 1 with sigmoid activation function to the [CLS] token to output the similarity score.

It also contains the code for predicting the quality score of the argument. Used the Arg-Ranker Datasetreleased by IBM covering 5,298 arguments where each argument was explicitly labelled for quality.For each argument in the dataset obtained the embeddings by concatenating the last 4 layers of the BERT model. The embedding vectors were passed as input to a hidden layer and a single output layer.Sigmoid activation was used in the output layer to output a quality score between 0 and 1
