# reddit-royalty

I scraped over 20,000 pages on Reddit to try to understand what helped a post get to the front page. I used a Random Forest in sci-kit learn as my model. I found that an author's 'karma' was one of the most predictive factors, and also saw that certain users kept getting to the top page within a small period of time. Given the numbers of users on Reddit, that was surprising, and I called these super users 'reddit royalty'. If I had more time, I would have focused more closely on following the trajectory of all of the posts of these supers users, to try and get a better sense of what was allowing this elite group to dominate the front page.

The notebook has the scrapers as well as my feature engineering and modeling.

The presentation is slides I used for my talk at General Assembly.

Below is the “pitch” I wrote about my work. 

## The rise of reddit royalty
(I felt as though a pitch was better than an executive summary, given the prompt)

Over the last 3 months, reddit.com has been the 4th most visited site in the U.S. The site is popular for its never-ending stream of fresh memes, but also for its community feel. Its old-school aesthetic harkens back to an internet that is slowly disappearing: community-regulated, no censorship, and non-hierarchical. These attributes used to be associated with the internet at large, but as titans such as Google and Facebook control more of the internet, and as governments and advertisers becomes more interested in regulating the types of content that appears, reddit appears to fight against the current. But even in reddit, there does appear to be a favored class that have undue influence on the site. 

I propose an article profiling this group of superusers and their influence on reddit's front page. I would track all posts created by these users over a month and compare them to a a random set of posts from Reddit's "new" page. I would interview and profile some of these superusers, using their stories to explain reddit's evolution over time. Lastly I would place the increasing hierarchy of reddit in the context of broader overall shifts in towards more sanitized and hierarchical structures on the internet and mobile apps.

My preliminary research suggests that these reddit super users do exist and are very influential.Users who frequently were in the top 350 "hot" posts over the week that I scraped the website had nearly double the median number of comments (19 versus 11) and average (132 versus 62). I used random forest modeling to strengthen the claim that who a user is as determined by their post and comment "karma" raises the likelihood of having a higher number of comments. 

While reddit is certainly still more democratic, open, and community-oriented than much of the other popular internet giants, there are still a group that has a lot of influence over how the majority of users view the site. It's time to uncover the reddit royalty. 


from sklearn.externals import joblib
jobmodel = joblib.load
“wnv_ predict_