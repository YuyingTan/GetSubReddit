# GetSubReddit
I wrote this python code for my research. By using PRAW library, the code can collect the latest hot posts/comments/meta data from selected subreddit communities. This code can help people who want to learn collecting data from Reddit using Python and API.

# How to use
You can open the Scraping Reddit.ipynb in your Jupyter Notebook to see how it works, I wrote notes for every part of codes. I also described the general steps in the code as follow:

### Step 1: Find the subreddit community you want to investigate.
Before collecting data, you need to find which subreddit community you want to investigate. It can be very difficult to find the community relevant to your research topic. One popular way to find relevant subreddits is by searching keywords, however, this is very inefficient. I found that on Github, here is a Map of Reddit tool to help you find the subreddit community https://anvaka.github.io/map-of-reddit/?x=145246&y=454606&z=3257.015516997539

It is very helpful, because it is actually a social network map of Reddit. Similar to how you use Google map, on the Reddit map, you can search keywords to find the relevant communities, and the closely related communities. More details of the map you can check the above link.

After selecting the subreddit community, you can start collecting data from the community as following. 

### Step 2: Create your own Reddit developer account 
Go to https://www.reddit.com/prefs/apps/ and register then get your secret, id etc., information

### Step 3.1: Create a function to get posts and meta data from the subreddit community you choose in Step 1.
In the Scraping Reddit.ipynb file you can find a function that I created to get posts and meta data related to each post (user id, username, subreddit, title, score meaning the number of upvotes for the submission, number of comments, self-text, created time, pinned, total awards received, upvote ratio, url of the post).

### Step 3.2: Create a function to get not only posts and meta data, but also the comments from the subreddit community you choose in Step 1.
In this step I collected not only the posts and meta data as mentioned in Step 2.1, but also the comments under each post. The meta data of the comment include comment id, comment parent id (which help you map with the post), comment body text, comment link.

### Step 4: Call the function to collect data from Reddit
In the Scraping Reddit.ipynb file you can see example of how to call the function and the result data. 

After finishing all the steps, you can get the collected data stored as .csv file.




It is first time I share some codes on Github, if anything unclear or inappropriate, welcome contact me for improving!

Thank you for your support!
