---
layout: post
title:  "Social Media Study Case 2"
date:   2019-12-17
excerpt: "Topic Modeling using R to find the potential trend of food"
project: true
tag:
- Social Media 
- R
- potential trend of food
- Facebook posts
comments: true
---

    
## Introduction
In this case study, In this report, the potential trend of food was found by Facebook posts incorporating the frequency of ingredients of food. Therefore, in order to obtain the potential food trend, the frequency of different ingredients words over 60 months is investigated to predict the pattern of certain words. 
      
      
## Data
There is a big dataset includes a txt file of ingredient words and Facebook post in every year from 2011 to 2015, 5 years in total.

## Methodology
Firstly, I used `ingredient.txt` as the target list to extract various words inside the data (Facebook posts) and integrated them into a data frame. 

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LajthsWAtRh*OVE*STb8ArKLQfowZrdG.cnAhImnAwkrG9DehWr5eSzHI5Ta8t9N8RItDYetvH2QgO.Q6XhVaSJU!/r" width = "300" height = "200">

Secondly, the names of months and years are obtained from the row names of the data frame. Thus, I could utilize them to make the aggregation function, which was used to find the frequency of different words.

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16Lamm*YIymrvSUTGelLh51.Q0g3vHw28Eo8hurHq26r7aIkHW0KWVHuf9MaHjc.lDULJfQ3YIIda*iSUDJkYXHzRQ!/r" width = "300" height = "200">

Finally, a function was constructed to plot time-series graphs of different words. 

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16Lap5axf8v2yHsTSYY2e9YunuOTi5y04aNh12iyuoBdN3Jl9xgkiZzp6tCQeSeW5ulrRSgepai72DQ1Kxo5bl8p8M!/r" width = "300" height = "200">


## Validation
The trends of `Cauliflower Rice`, `Vegetables Noodles` and `Pumpkin Pie` were used to test the effectiveness of a method. It is worth mentioning that here I plotted individual words such as `Cauliflower` and `Rice` firstly, and compare plots of them to find a common trend. Hence, I could discover the trends of two words or more together.

### Cauliflower Rice
In general, the demand for cauliflower rice has been growing steadily over the past few years largely due to consumers’ desire for a healthy alternative to white rice and gluten-filled grains. Therefore, both words showed upward trends. They also revealed  a similar trend after 2015 because of the expanded the cauliflower line. Consumers are more likely to get `cauliflower rice` so that they will mention more times about cauliflower rice on Facebook. 

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LaoIpdx6zUOQ6u0gm3trUl2DTSuilKz6uUTj17B3GOnc5OI6rLIKnyX5Z581LSzZ8Uk1NCaR*pDqWVeGh2CXWrsU!/r" width = "300" height = "200">
<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LalaGtfXyizi7W0l1yBSWyY68PCwixAFfXzJuNLwHcxad9SaGzO3lE.7XigUNvgq9VgaqcSRO0zYyoeZOIVmC7*s!/r" width = "300" height = "200">

### Vegetables Noodles
In January 2015, Vogue indicated that vegetable noodle was good for people so that there were large increases of Facebook posts of both words of `vegetables` and `noodles`.

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16Lau.wKID*zJmdEJqtVRbgnw3FiHAxzb2cm4tGzudTbX2DN.PzgRnt3uaLmnGi68b*XCkPpAKxBLga3tbkBWcHHgI!/r" width = "300" height = "200">
<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LaoqCk1NDkIRdBuNyzZ5PlXPdpwHa091gQlGw7AO.sCnrr0TZEFZMjOIdo9*0D6Qf7OuEUcJyEme1EcymUj1Eym0!/r" width = "300" height = "200">

### Pumpkin Pie
During Thanksgiving, the `pumpkin` and `pie` occur together to a large extent. The trend was much more obvious for pumpkin might because it is a special word that is highly used in Thanksgiving Day. 

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LajJ6*nlNNK5249s2dIN*fi4yWnqdiugMmKppRGmw9owT85j4oFcoHW2roXuxYHtLO0dFNludNVKLWMsqyOnqcLU!/r" width = "300" height = "200">
<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16Laj12pbg1lgW9WPScU7umCZD5QlfzwJOQdyOGe8onj0eAkcHxuAefNIaU8MBN*e.i.wNSRPGJFmIEzlwKGxeWHLE!/r" width = "300" height = "200">

## Further Improvement 

Although the figures can accurately show the trend of different words in general. There are still a large number of drops or spikes that are hard to be explained. Thus, it means that the method was not precise enough. Next time, the co-occurrence matrix can be tried to test whether a better result can be derived through this method.

## Specific Content in GitHub

url: <https://github.com/XinyanCai/Social-Media-Study-Case-2>

