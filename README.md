# Twitter API Reciprocal Friends

Using (crawl_followers()) function from the Cookbook, find the reciprocal friends in the network. 

Select a ‘starting point,’ i.e. a user on Twitter, which could be yourself or somebody else. Retrieve his/her friends, which should be a list of id’s, and followers, which is another list of id’s, perhaps using the get_friends_followers_id() function from the Cookbook, or your own program if you prefer. Note: When you use get_friends_followers_id() or its equivalent, you are allowed to set the maximum number of friends and followers to be 5000 (but no less), in order to save API calls, and hence your time.

![Network](https://user-images.githubusercontent.com/28322834/123499089-39a00880-d602-11eb-8d39-ddd8d1289b74.png)


Use those 2 Step to find reciprocal friends, which is yet another list of id’s. From that list of reciprocal friends, select 5 most popular friends, as determined by their followers_count in their user profiles. Repeat the process for each of the distance-1 friends, then distance-2 friends, so on and so forth, using a crawler, until you have gather at least 100 users/nodes for your social network.

Calculate the diameter and average distance of your network, using certain built-in functions provided by Networkx.
