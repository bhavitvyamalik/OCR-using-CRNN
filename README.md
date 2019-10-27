# OCR-using-CRNN

Essentially what CRNN does is it integrates feature extraction, sequence modeling and transcription into a unified framework. 

Advantages of this technique:
1) End-to-end learning is possible.
2) Sequence data of arbitrary length can be processed because of LSTM which is free in size of input and output sequence.
3) There is no need for a detector or cropping technique to find each character one by one.

Inspiration: https://arxiv.org/pdf/1507.05717.pdf

Dataset used: The Street View House Numbers (SVHN) Dataset  

You can read more about CTC model in Keras here: https://arxiv.org/abs/1901.07957. It is quite an interesting paper in which they have explained how to perform the Connectionist Temporal Classification (CTC) in a transparent way.
 It consists of three branches made of Keras models: one for training, computing the CTC loss function; one for predicting, providing sequences of labels; and one for evaluating that returns standard metrics for analyzing sequences of predictions.


Blog explaining CTC loss in detail: https://theailearner.com/2019/05/29/connectionist-temporal-classificationctc/
