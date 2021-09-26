# comment-verification

This repo has two different approches to identify spam comments based on [digikala](https://digikala.com) comments.

digikala is the largest online market in Iran.

I solved this challenge by implementing multinomial naive bayes approach without using NLP libraries.

on the other approach, I used TF-IDF method to vectorize statements, and then by using logistic regression library, comments classified to target classes which are either spam or not spam.

the dataset has 160000 entry in train datas which each of them is a seperate comment. For every comment, there are some information namely, id, a title, a comment, a rating, and a verification status.

the test datas consist of 20000 comments.

### visualization by generating a world cloud
for a better understanding of data and do some exploratory data analysis to have an idea of the distribution of words, I generate word cloud for this dataset.

![wordcloud](https://github.com/mohamadreza99/comment-verification/blob/main/wordcloud.png)

Everyone who enjoys to using this data for the sake of challenging their solutions, there is a jar file that you can use it to calculate your final accuracy.
if your results csv file's name is res.csv, you can use this in the following way : 
```
java -jar CommentJudge.jar res.csv
```
