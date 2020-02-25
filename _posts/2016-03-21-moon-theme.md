---
layout: post
title:  "Machine Learning Challenge"
date:   2016-04-06
excerpt: "An efficient approach using python to predict default risk"
project: true
tag:
- credit 
- risk
- python
- machine learning
comments: true
---

    
## Purpose
* Develop a predictive model and a decision support system (DSS) that evaluates the risk of Home Equity Line of Credit (HELOC) applications.
      
      
## Data Collection & Cleaning
* Collect Data from the [FICO](https://community.fico.com/s/explainable-machinelearning-challenge)
* Utilize `Pandas` to clean data
* Remove Column with more than 90% omitted data
* Modify other omitted data by Imputer strategy `mean`
* Divide whole data frame into `Train_set` & `Test_set`

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LamFgsLsCkC5MtzbhF8aOBEUYy7h3t6o6JFcHwoOXvX5YyZWNGr1eicRyDyZEHuHHOVJ7WqLCGhw2lXkV7lQJwng!/r" width = "300" height = "200">


## Default Risk Prediction Using Machine Learning Algorithms
**Five Algorithms**
* Random Forest
* Linear Model
* Support Vector Machine
* Bagging
* Boosting
* Neural Network

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LaneuZPDGZK30pGlNOUp3aUPppeQroPWWusjsbhPolR7fXjVRxJMZvgB5MaipDJ21ZlwFmERQY94sc2SS9WFNnZg!/r" width = "300" height = "300">
<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16Lav.FXSYSziyvcBnUCZ7xpC9FU*sREf1fy9VfICvHKJu3ka7D5I0hL.uqVmnR2U2iKtzTo4LzKErSL0be8lhPRTc!/r" width = "300" height = "300">
<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LanBHooZI2hpcyrtoTEQTNyVN9KqWBdNWsKhDgw9qE4LsQyGj5AnKuHl61RV4rzL3Aq1xLwwh.DUG2j8WV8yBLK4!/r" width = "300" height = "300">

## Interface Build
* A user friendly platform to enable bankers to better access each customer's default risk
* Weakness: Long Running Time

<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16Laorq5XcnI8cTO5lJ1*fVFpCXh*xvtA9orTDXvLE8MdwKwGxCQ2Pa2ig.BsXpNpDBSINIkrwaMPGU6.XF*oq4Z1g!/r" width = "300" height = "200">
<img src="http://r.photo.store.qq.com/psc?/V10MU7Rq18V88Z/zxjvJoYbvlQPq4wKS16LahFJLzqghaqRFMe6XUsoITxQRjIexwZQ6B5op42Ch0np2MFemv1SxIPj5tqdFKfgrRonnAkF.2ZliDA3TMi8*eY!/r" width = "300" height = "200">


### Specific Content in GitHub

{% highlight yaml %}
url: https://github.com/XinyanCai?tab=repositories
{% endhighlight %}

#### reading_time

Set true to show reading time for posts. And set `words_per_minute`, default is 200.

#### logo
Your site's logo. It will show on homepage and navigation menu. Also used for twitter meta tags.

#### background
Image for background. If you don't set it, color will be used as a background.

#### Google Analytics and Webmaster Tools

Google Analytics UA and Webmaster Tool verification tags can be entered in `_config.yml`. For more information on obtaining these meta tags check [Google Webmaster Tools](http://support.google.com/webmasters/bin/answer.py?hl=en&answer=35179) and [Bing Webmaster Tools](https://ssl.bing.com/webmaster/configure/verify/ownership) support.

#### MathJax
It's enabled. But if you don't want to use it. Set it false in  `_config.yml`.

#### Disqus Comments
Set your disqus shortname in `_config.yml` to use comments.

---

### Navigation Links

To set what links appear in the top navigation edit `_data/navigation.yml`. Use the following format to set the URL and title for as many links as you'd like. *External links will open in a new window.*

{% highlight yaml %}
- title: Home
  url: /

- title: Blog
  url: /blog/

- title: Projects
  url: /projects/

- title: About
  url: /about/

- title: Moon
  url: http://taylantatli.me/Moon
{% endhighlight %}

---

## Layouts and Content

Moon Theme use [Jekyll Compress](https://github.com/penibelst/jekyll-compress-html) to compress html output. But it can cause errors if you use "linenos" (line numbers). I suggest don't use line numbers for codes, because it won't look good with this theme, also i didn't give a proper style for them. If you insist to use line numbers, just remove `layout: compress` string from layouts. It will disable compressing.

### Feature Image

You can set feature image per post. Just add `feature: some link` to your post's front matter.

```
feature: /assets/img/some-image.png
or
feaure: http://example.com/some-image.png
```    
 This also will be used for twitter card:

![Moon Twitter Card](https://cloud.githubusercontent.com/assets/754514/14509719/61c5751c-01d6-11e6-8c29-ce8ccad149bf.png)

### Comments
To show disqus comments for your post add `comments: true` to your post's front matter.

---

## Questions?

Found a bug or aren't quite sure how something works? By all means [file a GitHub Issue](https://github.com/TaylanTatli/Moon/issues/new). And if you make something cool with this theme feel free to let me know.

---

## License

This theme is free and open source software, distributed under the MIT License. So feel free to use this Jekyll theme on your site without linking back to me or including a disclaimer.
