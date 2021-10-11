# Multi-Class-Text-Classification
Performing multi class classification on tweets using different models (BERT, LSTM &amp; GRU) and comparing the results.
#### Data
The data is prepared by preprocessing and formatting the [kaggle dataset](https://www.kaggle.com/datatattle/covid-19-nlp-text-classification) which consists of corona virus related tweets segregated into 5 classes namely, Extremely negative, Negative, Neutral, Positive and Extremely Positive.

### Conclusions

<p align='center'>
<img src='https://github.com/kushagra801/Multi-Class-Text-Classification/blob/main/accuracy_comparison.png'>
</p>

<p align='center'>
Accuracy Comparison
</p>

<p align='center'>
<img src='https://github.com/kushagra801/Multi-Class-Text-Classification/blob/main/loss_comparison.png'>
</p>

<p align='center'>
 Loss comparison
 </p>
 
For training small_bert/bert_en_uncased_L-4_H-512_A-8 model was used in addition to comparable LSTM and GRU models with 4 hidden layers. As we can see from the accuracy and loss comparison graphs it takes longer time to fine-tune the bert model compared to the other two but the generalisation of the model on unseen data is better as compared to LSTM and GRU. LSTM, on the other hand starts to overfit the data as the training accuracy goes very high and the training loss gets quite low only in a few epochs. 

BERT outperforms both other models with a test accuracy of 91.70% (the test accuracy mentioned for all models is averaged over 3 test accuracy outputs).
While LSTM and GRU have similar performance with test accuracies of 88.10% and 88.17% respectively.

 


