<b><font color="#6F6F6F" size="25"> Is machine learning the best solution to text mining? <font></b><br>
<b><font color="#6F6F6F" size="25"> What if graph theory beats it in both time and space complexity?<font></b>

<font size="10">
The answer is obvious, definitely not. The graph theory is definitely an underestimated data structure, compared to all that hype of machine learning. First, let's talk about what this project is and later you would realize why graph structure works better. Graph theory turns out to beat supervised learning in both time and space complexity. 

This project to is designed to be integrated into my scraping script called MENA news feeds (https://github.com/tattooday/web-scraping/blob/master/MENA%20News%20Feeds.py). Initially, the script would scrape news titles from different main stream websites (so-called fake news, lol) including BBC, CNN, Reuters, Al Jazeera etc. All these scraped news titles, links and preview images would be concatnated into one HTML email and automatically send it to my inbox every morning. After a couple of days, I realized that many websites were actually reports the same story but in different titles and preview images. It was a totally waste of energy and time to read these similar contents over and over again. And not every piece of information was worth my time to read. Some stories such as 'British Iranian woman got put in jail' was not exactly business related (I'm sorry, it is still a great story though). Couldn't I find a way to create a filter to extract the key information?

The first thing came to my mind, of course to anyone, was machine learning. We could build up a classifier to determine which one is key information. A simple Naive Bayes Multivariate Event Model would do the trick. The methodology is basically based on the assumption that when certain key words such as 'oil','crude','south pars' and 'LNG' come together in a title, the title is more likely to be oil business related. It turned out that Bernoulli Naive Bayes Classifier worked pretty well for key information screening. The accuracy was always capped at 70 to 80 percent. It could be improved by building up a better stopword list. The downside of this is the time complexity. It is always the issue of supervised learning even if it is generative learning. The default sklearn package needs to calculate the conditional probability of each word in the vocabulary list repeatedly when making a forecast. 
<font>

![alt text](https://github.com/tattooday/graph-theory/blob/master/Text%20Mining%20project/preview/original.png)
![alt text](https://github.com/tattooday/graph-theory/blob/master/Text%20Mining%20project/preview/bfs.png)
![alt text](https://github.com/tattooday/graph-theory/blob/master/Text%20Mining%20project/preview/target.png)
![alt text](https://github.com/tattooday/graph-theory/blob/master/Text%20Mining%20project/preview/result.png)
