# CS410 MP3---Part 2

In this part, you will develop a classifier and participate in a classification competition. Your classifier will be evaluated using F1 scores on 2 datasets: metamia dataset (created from metamia.com),  MP3.1 Analogy dataset collected and annotated by you and your classmates. 

**Note: MP3.1 Analogy dataset will be released later around Nov, 23. But, you can already start working on the Metamia data**

**The evaluation results will be displayed on the leaderboard on LiveDataLab. Only your latest submission results will be displayed here.**

## Due: Dec 15, 2023 at 11:59 pm CDT


## Competition Tasks

[*bert_finetune.ipynb*](https://colab.research.google.com/drive/1U0-Lq1GqJRVaD5IVqMYoTHnQQjWv0q_O?usp=sharing) contains some starter code to finetune a [BERT](https://huggingface.co/docs/transformers/model_doc/bert) model on the training set and generate predicted labels for the test set.

1. Download both the Metamia and MP3.1 Analogy datasets from [here](https://uofi.box.com/s/aa1yhe7y93yllkvzrmufxtyzexxa5lt6)

2. Train or fine-tune models on the respective training sets. 

If you are using [Google Colab](https://colab.research.google.com/), the starter code provides an example of reading the data from your Google drive. Make sure to create a copy of the notebook and then modify it as needed. Also, you need to upload the data to your Google drive.

You are free to use any classifier (Hint: The web pages are really long, so models suitable for long document classification (e.g., [Longformer](https://huggingface.co/docs/transformers/model_doc/longformer)) might work better) and fine-tune various hyper-parameters (e.g., learning rate, number of epochs). We recommend you start by experimenting with learning rate and number of epochs.


3. To see how well you perform in the leaderboard, you need to run the prediction code on the test sets of both the datasets. For metamia dataset, save the results as `metamia_results.csv` and for mp3.1, save as `mp3.1_results.csv`. These two files must be located in the root folder in your repo, i.e., it should not be under any sub-folders. 


There are no restrictions on the number of submissions.

## Grading

The leaderboard shows details of the performance (F1) on the test sets. You will be graded based on the Metamia dataset only. You will receive full credit as long as you beat the baseline on the Metamia dataset. The last column on the leaderboard, "Completed", indicates whether you completed this requirement or not (1 or 0).  

## Bonus: Top ranked in Classification Competition Leaderboard

Try to get a top position in the competition leaderboard. The higher your rank is, the more extra credit you will receive. The rank is based on "Average F1", which is computed as 0.7* Metamia F1 + 0.3 * MP3.1 Data F1.

Our grading formula for the competition is max(0, 5-(Rank-1)/10) where Rank is the position of the student. This means that about 50 students will receive an extra credit greater than 0. Students with the same score will receive the same extra credit.

You will not immediately see the extra credit score on Coursera since it depends on your final rank in the leaderboard when the deadline is over. We will add your extra credit score on Coursera later.


