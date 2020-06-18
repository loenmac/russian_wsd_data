# Generating Training Data for Word Sense Disambiguation in Russian
The repository contains algorithms concerning the task of generating training data for word sense disambiguation in Russian.

Classification algorithm, training and test procedures are heavily based on: https://github.com/uhh-lt/bert-sense

Extracting ELMo embeddings trained by RusVectores team was performed with the help of this resource: https://github.com/ltgoslo/simple_elmo

To use this framework for compiling training collection for the WSD task, perform the following steps:

- preprocess your text data with scripts contained in Processing.ipynb
- train word2vec model on your preprocessed text data with scripts contained in Word2Vec_Training.ipynb
- extract monosemous relatives for the target polysemous words with algorithm implemented in Extracting_relatives.ipynb
- Test_Train_Collection_creation.ipynb is used to compile test dataset and train collection in xml-format. This format is used in repository https://github.com/uhh-lt/bert-sense on which we based our training and inference procedures.
