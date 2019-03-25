# Capstone-Project2
# High level description of project.
    The goal of this project will be to use unsupervised learning and dimensionality reduction techniques to discover "classes" of quotes in the Wikiquote and possibly other quote sources, and then to extract the most important features of the quotes in order to generate "meta-quotes". A "meta-quote" will be a synthesisis of all of these different quotes into a certain, overaching quote, that is essentially an "average" of what they all said. The idea is essentially to distill wisdom from many sources into one sentence, representing many different people. 
    
    The first step will be aggregating quotes from famous people, likely using
    Wikiquote. Wikiquote has 34,000 articles, which are divided into different subcategories. The categories include Films, Literary works, Occupation (of the quoted person), Proverbs, TV shows, and Themes.
    
    At the first iteration of the project, I would start with the 'Occupations' category, and begin with one occupation. For example, I would take "Inventors", which has 122 pages, and download all of the quotes across these 122 pages. In the final part of the project, however, I would want to take quotes across all occupations and merge them together for the analysis.
    
    The analysis will likely consist of a combination of NLP, unsupervised learning, and neural networks. The unsupervised learning will classify the quotes into their topics. The NLP will then be used to find the most important features of each topic, probably as some type of n-gram. I'm more hazy on the aspect of creating one quote that is representative of an entire group- the mechanical aspects of that may be challenging.
    
    As a subset of this project, I could also give a neural network quotes from a particular person or period, and see if I could train it to produce quotes indistinguishable from what it received. 

    If these things work, I would like to move up to using full texts from actual books. Quote databases are only a fraction of what people actually say. I would probably move by sentence, having the algorithm classify each sentence into a particular topic, and then have the neural network train on the new collection of "quotes"- really, just sentences. 
    
#What question or problem are you trying to solve?

    The problem is a bit like what motivated the Blinkist app. Blinkist is an app which takes books and has people read through them to 'distill' the main ideas in them into bite-size chunks. While I don't really agree with their approach, I agree that there is simply too much material and not enough time for us to read all the great works of history, finding the wisdom inside them and incorporating it into our lives. Thus, this project seeks to summarize many great thinker's thoughts on different topics. If they disagree on a topic, I hope to be able to distinguish between their viewpoints, perhaps using a sentiment analysis software. For example, on a particular topic like "Love", this may be split into 6 different viewpoints, each of which will be summarized with a single quote. 
    
    The goal of this is to help people access the wisdom of the ages without reading every single word of all of its pages.

    
#How will you present your work?

    I definitely would like to create an interactive website, where users can look for our algorithmically-generated "quotes" on whatever topic they may like. In the "About" section of the website, I would explain in detail how the app was created. 

#What are your data sources?

    While wikiQuote seems to be the most professional and exhaustive, there are multiple online sources of quotes. The Cambell County Public Library has 25,000 quotes. Downloading these and merging them with the WikiQuote Database could probably be its own project, so I will try to use the most easily available/ reputable data.   

#What’s your next step towards making this your project.

    Probably figuring out how to scrape WikiQuote, and Google Books for the second stage of the project. Really, the most important step, though, is to iterate through with a small set of quotes, to see whether I can actually do what I hope to- create quotes that summarize many great thinker's thoughts on a topic. 