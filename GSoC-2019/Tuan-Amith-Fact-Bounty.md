# Project Name
Fact Bounty

## Student Info
* Name - Tuan Muraad Amith
* Email - [ymuraad@gmail.com](mailto:ymuraad@gmail.com)
* University - University of Colombo School of Computing
* Github Profile - [https://github.com/root5533](https://github.com/root5533)
* LinkedIn Profile - [https://www.linkedin.com/in/root5533/](https://www.linkedin.com/in/root5533/)

### Project Abstract
Fact Bounty is a platform where the truth and validity of news is determined through crowdsourcing. The main objective is to spread awareness regarding fake news and with the help of visualizations, help users determine the spread of such news documents. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6365922036547584)

### [GSoC Project Proposal](https://summerofcode.withgoogle.com/serve/5052203209850880/)

### [GitHub Organization Repo](https://github.com/scorelab/fact-Bounty)

### [GitHub Personal Repo](https://github.com/root5533/fact-Bounty)

### [Commits during GSoC 2018](https://github.com/scorelab/fact-Bounty/commits?author=root5533)

### [Project Wiki](https://github.com/scorelab/fact-Bounty/wiki)

### Work Summary
During the GSoC period, I was able to complete the milestone of visualizing the rumour spread of a certain news item in tweets. Depending on a specific keyword, the relevant tweets, retweets and quotes are gathered and visualized in a graph that shows how many users have retweeted a certain tweet from a user and how many users have tweeted regarding the keyword.  

### What Covered
Following are the tasks that was completed.
* Created a Twitter app using the Twitter developer platform to allow searching and retrieving tweets from Twitter.
* Set up an authentication portal using oauth.io that will handle complex authentication flows in order to provide permission for client app to use user's Twitter account to retrieve tweets. 
* Authorize each user with Twitter app and save the tokens to prevent user authorization everytime user searches for tweets.
* Given a keyword, retrieve a maximum of 1000 tweets related to the keyword by sending multiple requests to Twitter search API.
* Generate and visualize a directed graph using sigmajs where each tweet represent a node and each edge represent the tweet was retweeted or quoted by a user. 
* Show twitter handle of user in each node label.
* Preview details of tweet and user that each node represent.
* Visualize a timeline graph of cumulative tweets against the time the tweets were created. 
* Animate the graph showing the progress of tweets and retweets with time.

Bug fixes and CSS styling of client side application was also carried out during the GSoC period.

### What left
* Set up a free authentication portal instead of oauth.io

### Reference
* SigmaJS - http://sigmajs.org
* Twitter API - https://developer.twitter.com/en/docs
* OAuth - http://docs.oauth.io/
