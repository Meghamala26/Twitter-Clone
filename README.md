# Twitter-Clone

## Introduction


This project uses the web socket at the Server and Client side to ensure 2-way communication
between the server and client(and other client applications).


• We have implemented the registration functionality for the users. As soon as a user is
registered, their status is set to online.


• Users can login or logout.


• Users can subscribe to other registered users.


• Every user, if online, can tweet or retweet.


• A tweet can be any of the following:


    – Have a hashtag.


    – Have a mention.


    – Have both hashtags and mentions.


• As soon as a user tweets something, their tweet gets updated to all of their subscriber’s
feed.


• For every tweet, the tweet is immediately parsed to extract the hashtags and mentions(if
any) present in it. If there is any hashtag present, a record of the tweetId where it was
mentioned is added in a hashmap. Same happens for any mentions present.


• When the tweets are shown in the user’s feed, the user also has the option to retweet some
of the tweets from the feed.


• An user also has the ability to search for any hashtags. The tweets which contain the
searched hashtag are shown on the user’s feed. In case the hashtag is not used in any
tweet yet, no tweets are shown.


• An user also has the ability to search for mentions. All the tweets where the user is
mentioned is shown on the user’s feed. In case he has not been mentioned in any tweets
yet, then we display a message saying "The user has not been mentioned yet."




## Steps to Run


Run Server : dotnet fsi TwitterWebSktServer.fsx


Run Client : dotnet fsi TwitterWebSktClient.fsx


## How to use


• To register user : Register, \<username\>, \<password\>


• To login: Login, \<username\>, \<password\>


• To logout: Logout


• To subscribe to another user: Subscribe, \<subscribedusername\>


• To tweet: Tweet, \<tweet_text\>


• To retweet: Retweet, \<tweetId\>


Note: tweetId is displayed with tweet on client feed


• To see all tweets on user’s feed: Query


• To query for hashtags: QueryHashtag, #\<hashtag\>


• To query for mentioned user: QueryMention, @\<mentionedUsername\>
