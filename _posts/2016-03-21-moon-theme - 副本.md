---
layout: post
title:  "Social Media Study Case 1"
date:   2019-12-23
excerpt: "A case study using R to find noncomplaint twitter posts"
project: true
tag:
- Social Media 
- R
- noncomplaint twitter posts
- airplane company
comments: true
---

    
## Introduction
In this case study, the types of Twitter posts incorporating noncomplaint and complaint were classified using the featured negative words. The judgment of Twitter posts types could help the airplane companies to identify customers’ attitudes towards their services, therefore leading to service improvements. The whole investigation aims to find noncomplaint twitter posts.  
      
      
## Data
There are two big datasets include the noncomplaint twitter posts and complaint twitter posts which are utilized to build the model. After that, another data with mixed types could be classified by the model built before.

## Methodology
Firstly, I obtained data from the SQL server and store it as a local file called ‘final.csv’. Also, I read different files to R. 

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16Lana*Zrf3rFvkJMW5gFe0eKcpyxLvARyLL6c1hoC*cHq0lHo9r4D8IoZ7laMgLCPstirY2H6oujjhllMaqeXeTdo!/r" width = "300" height = "200">

Secondly, I extracted complaint words from only the complaint dataset because the complaint words were more radical so that is could be easier to classify the complaint posts and noncomplaint posts. Here I specifically extracted adjectives, nouns, advs, and verbs from the complaint dataset and the most useful words belonged to adjectives. It is reasonable that people often use adjectives to express their emotions. 

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LaoAfNo9torlGcP90vUvAsaJ3wkb7zNOkfvOF1VfxGseSYf.XckkIF*R1ppck3fB7oRuRdLKXppEase5IL3RWUEo!/r" width = "300" height = "200">

Thirdly, I found that some words extracted from complaint posts are misleading or meaningless such as `good` and `able`. Therefore, there was an important step that I wrote the words into a local file for the further edition by hand. 

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LasTufPz1d5B9Keu.R.AsQIKMGwTeYf.Iu1hy2Spk83bWKKqJks3eZULxv4.jRSvMbJfTZIKugGZd4kdbJr*h.kQ!/r" width = "300" height = "100">

Furthermore, according to the combination of the complaint and non-complaint datasets, I derived X and Y using the complaint words I modified. It is also worth mentioning that I decided on the classification (Y) in terms of `rowSums`.

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16Lahf9iWKwLtCFsaEP9oGhhLHfVWEjXT1bR.vE1UtF7yO9zboXfT1A0zPD*92IaTToTcJ93Fkm.rx5ZT*6N5h3xag!/r" width = "300" height = "200">

In order to find `X2` of the dataset with mixed posts types for further prediction, I also created `dtm` of this dataset. 

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LaqzjAUSeECwyfxEQJ58rGZEyF6K1p4khf0WanotCCujbAOJSduvvZGgWjSiLEwu4qMGxN4wz3sL7g60O00yttyM!/r" width = "300" height = "200">

Finally, in order to build random forest more successfully and easily, I used python to do final model building and prediction. 

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LaoG..BZq.U3OIU80sMv4C49XHRfMMNYIjD2TbgyFJLnBbOpRpk13ndTfoIIKlrpoksyn8oHt7gNOBN5btY3fZCQ!/r" width = "100" height = "100">
<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16Lalw8XAPYsmz9pM2ynnWgRdOVPO64HyNBKnl*cgARuXVzAkoqNxvOHxaRZdgvhsz9Eq*wQwKk0a7WdlKqx6QwOXU!/r" width = "300" height = "400">

## Validation
In total, I obtained 143 non-complaint twitter posts and the accuracy is around 0.7 which is not bad. Therefore, it indicates that my model is precise in general. 

## Further Improvement 

Although the model can accurately classify the types of twitter posts. There are still a large number of posts that are hard to be separated. Thus, other models such as SVM, bagging, and boosting can also be tried. Meanwhile, it is also significant to extract more meaningful words among the complaint file, which is beneficial for prediction. 

## Specific Content in GitHub

url: <https://github.com/XinyanCai?tab=repositories>

