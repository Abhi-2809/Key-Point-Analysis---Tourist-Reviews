# Key-Point-Analysis/TouristReviews
This code contains the code for Fine-tuning the BERT model to calculate the similarity score between two sentences. The Argument and Key-pointwere given as the input along with special tokens [CLS] atthe beginning and the [SEP] token between Argument and
Key-point. Trained the model for 3 epochs by adding a linear fully connected layer of size 1 with sigmoid activation function to the [CLS] token to output the similarity score.
