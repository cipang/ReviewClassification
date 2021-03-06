# ReviewClassification

[Pandas](https://pandas.pydata.org/) library is used to read and resize to a balanced dataset.

* To generate the embeddings, following libraries are used.
  - [word2vec](https://radimrehurek.com/gensim/models/word2vec.html) from Gensim
  - [sent2vec](https://github.com/epfml/sent2vec) library
  - [bert-as-service](https://github.com/hanxiao/bert-as-service)
  
  - pre-trained models can be download from
    - word2vec : [GoogleNews-vectors-negative300.bin.gz](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit)
    - sent2vec: [Pre-trained models](https://github.com/epfml/sent2vec#downloading-sent2vec-pre-trained-models)
    - BERT: [BERT-Base, Uncased](https://storage.googleapis.com/bert_models/2018_10_18/uncased_L-12_H-768_A-12.zip)

* [Yelp!](https://www.yelp.com/dataset/) and [Zappos](https://ppgweb.s3.us-east-1.amazonaws.com/share/reviews_shoes.tar.bz2) datasets are used for the analysis in the project (full datasets are included in the link).
* Following datasets are csv files containing reviews with their corresponding embedding vectors and labels, which can be used for training and predicting without further processing. (The naming conversion except Yelp.csv and Zappos.csv is as follow: [embedding modeol]-[training corpus]-[training or test and validate])
  - [Yelp!](https://drive.google.com/drive/folders/1bVIy2jpYiLmOkzAkxJhcqPx4iTi91U7p?usp=sharing)
  - [Zappos](https://drive.google.com/drive/folders/1oFkUZtpG34y-Os4AB_RP0eRAEIF5nMrJ?usp=sharing)
  
  all datasets used will be fully uploaded by 19.05.2020

* Following Jupyter Notebooks are included:
  - <b>s2v-bert-tfif.ipynb</b>
    - This Notebook is used for classification of s2v, BERT and Tf-idf embedding with either Neural Network classifier or SVM
  - <b>word2vec.ipynb</b>
    - This Notebook is used for classification of w2v with either Neural Network classifier or SVM
  - <b>accuracy.ipynb</b>
    - This Notebook includes a method to help calculated class wide accuracy from a confusion matrix.
  - Unitility Notebooks are included in the util folder, which helps to generate and read various embeddings.
  - Detaile instructions are included in the Notebook
 
Two python files are included to help with the embedding processing and classification. Parameters in the <b>NeuralNetClassifier.py</b> can be adjusted for further testing.

