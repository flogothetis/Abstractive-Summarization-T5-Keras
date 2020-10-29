# Abstractive-Summarization-T5-Keras

This abstractive text summarization is one of the most challenging tasks in natural language processing, involving understanding of long passages, information compression, and
language generation. The dominant paradigm for training machine learning models to do this is sequence-to-sequence (seq2seq) learning, where a neural network learns to map
input sequences to output sequences. While these seq2seq models were initially developed using recurrent neural networks, Transformer encoder-decoder (T5) models have recently
become favored as they are more effective at modeling the dependencies present in the long sequences encountered in summarization.


## Implementation details
Abstractive summarization is a hard task, since long-dependency preserving is a demand. Furtermore, due to the hardness of the task the summarizer must be trained on 
large labeled datasets with powerful hardware. For that reason we levarage T5 model that is pretrained on similar summarization tasks, so we need to spend a few training 
epochs to achieve great results. T5 is consisted of the deep transformer blocks ( encoder-decoder) and uses SentencePiece algorithm for tokenization. Sentence piece is applicable for any language as it transforms all the characters to a normalized UNICODE world (including spaces). 

Hugging face's T5 pretrained model is fine-tuned on a small dataset from CNNDaily Mail.

<img src = "https://paperswithcode.com/media/methods/new_text_to_text.jpg" />


# Test it ..!
Change the text of the final notebook's cell to produce the summarization for your own text

## Run on Google colab
1. Open Google Colab
2. Load .ipnb file
3. Set hardware to TPU
4. Run all cells


