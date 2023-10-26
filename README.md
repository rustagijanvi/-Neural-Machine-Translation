# Neural Machine Translation Project
Neural Machine Translation (NMT) is a sophisticated task in natural language processing that utilizes artificial neural network models to translate text from one language to another. This project is designed to demonstrate the implementation of a basic NMT model for French-English language translation using a dataset obtained from [http://www.manythings.org/anki/](http://www.manythings.org/anki/). The main objective is to showcase the process of building an NMT model and evaluating its performance using the BLEU (Bilingual Evaluation Understudy) score.

## Project Steps

1. **Data Preparation:** Downloaded the dataset as a zip file and extract it into corresponding text files. These files contain tab-delimited bilingual sentence pairs in French and English.
2. **Data Cleaning:** Cleaned the text by removing non-printable characters, punctuations, and non-alphabetic characters. Convert all text to lowercase to ensure uniformity.
3. **Data Splitting:** Split the cleaned data into training and testing sets.
4. **Tokenizer Creation:** Created separate tokenizers for both the source (French) and target (English) languages to prepare the text for model training.
5. **Encoding and Padding:** Encoded and pad the input and output sequences according to the tokenizers and maximum sequence lengths.
6. **One-Hot Encoding:** Converted the output sequences into one-hot encoding for effective prediction.
7. **Model Definition:** Define the sequential model with an Encoder and a Decoder.
8. **Encoder Configuration:** Configured the Encoder with an Embedding layer for training word embeddings and one or more RNN/LSTM layers for sequence processing.
9. **Connection with Decoder:** Used the RepeatVector layer to connect the Encoder with the Decoder.
10. **Decoder Configuration:** Configured the Decoder with one or more RNN/LSTM layers and a TimeDistributed Dense layer for output generation.
11. **Model Training:** Train the model on the prepared training data, experimenting with various hyperparameters such as epochs, optimizers, and batch sizes for optimal results.
12. **Evaluation:** Utilize the NLTK library's BLEU score to evaluate the model's translation accuracy.

## Future Improvements

- Explore advanced NMT architectures, such as attention mechanisms and transformer models, for enhanced translation performance.
- Experiment with larger datasets and additional languages to broaden the scope of the NMT model.
