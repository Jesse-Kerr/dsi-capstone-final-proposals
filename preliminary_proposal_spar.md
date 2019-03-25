# Capstone-Project-4
# High level description of project.

The Spar app (stylized SPAR!, see (https://getspar.com/)[here]), is a "social
habit-building platform". SPAR! users join 'challenges' created by other SPAR!
users, such as "Go the Gym 4X a week" or "Meditate 2X a day". They then have to 
document that they actually completed the task by posting 1 minute videos of
them doing it (i.e., being physically in the gym, or getting ready to meditate). 
If they miss any videos (i.e., only check-in 3X a week or 1X a day,
respectively), they are charged a penalty (between 5-20 dollars for each missed
check-in (this value is different for every challenge.)) This penalty goes into 
the 'pot', and at the end of the challenge (lasts between 2 weeks to 6 months), 
those who haven't missed any check-ins split the earnings.

As a SPAR! user myself, I've found that the bottleneck in the process is finding
new challenges. Currently, one has to scroll through all of the open challenges
to find one he or she is interested in. Challenges are only open to new users
during the first 24 hours, meaning they go up and then quickly close, making 
it easy to miss one. Therefore, I want to build a recommendation engine for 
SPAR!, which will use a user's history to recommend relevant challenges to him/ 
her. 

Along with looking at what challenges a user has done, I also plan to look at
their earnings/ losses in each challenge, their engagement in the challenge
(measured by # of comments in the chat area), the details of the challenge (size
of penalty for missed check-in, frequency of check-ins, and duration of 
challenge), and details about the user (their city, bio, and potentially
Instagram account, which is often linked). 

These factors may have predictive power over what challenges a user decides to
do. For instance, if they lose money in a previous challenge, they might not
want to return to one that is similar to it. Conversely, if they're very engaged
in the challenge discussion, they might be more likely to return to a similar 
challenge. And they might prefer challenges with certain details, such as lower 
penalties and less frequent check-ins, which could also influence which 
challenges they choose to do. User details such as city and bio may be helpful 
to recommend challenges to new users with no challenge history.

The techniques I expect to use in this project are NLP and an algorithm like
logistic regression or boosted decision trees. While SPAR! already splits the
challenges into categories, I want to use NLP to make these categories more
granular. NLP could also be used to interpret the user's bio to extract their
interests from it. The boosted decision tree or logistic regression algorithm
will be used to classify new challenges with a "predicted proba" that the user
would do it, based off of what we know about the user. 

# What question or problem are you trying to solve?

I want to see if I can predict whether a user will repeat a certain challenge,
based off of their history and their performance in previous challenges similar
to it. If you lose money on a challenge, will you try again, or not? Do users in
certain cities prefer particular types of challenges? What challenge duration is
most popular in the app? What is the average earnings per challenge? What is the
average earnings in challenges in particular topics? Can we predict the 
challenges a user does from the interests expressed in their bio? 
What kinds of challenges are most popular? There are a great deal of questions 
that I can answer with this data, which makes it extremely exciting. 

This will also solve a problem for SPAR!, the problem of finding new challenges.

#How will you present your work?

In the long term, I want this feature to be implemented in the SPAR! app.
However, this will probably be outside of the scope of the capstone project,
considering that their app is on Rails, which I don't know. 

For the capstone presentation, I would like to write it up as a Medium article, 
with lots of EDA visualizations, depictions of the algorithm, and graphs of 
feature importance. And if SPAR! allows it, I would also want to make it a
stand-alone, interactive website that explains the analysis. 

#What are your data sources?

Specified above. 

#What’s your next step towards making this your project.

I've emailed SPAR!, and their executive director told me they are "open" to the 
project. I followed up with a description of the exact data I need and I'm 
waiting to hear back about that.
