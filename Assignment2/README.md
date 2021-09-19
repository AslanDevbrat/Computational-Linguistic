# Assignment 2
## language Modeling
This Repository contains contain two files 
	

 - Report of Assignment 2.pdf : this contain the report and answer to the questions asked.
 - Assignment 2.ipynb : contains The python code for the same. No extra lbraries other than Pandas was used.

This assignment was on Language Modeling

## Assignement discussion
Consider the following Mother Goose nursery rhyme(it is a string of words converted to lower case and
all punctuation marks have been removed). This is our training set.
\<s> peter piper picked a peck of pickled peppers \</s>
\<s> a peck of pickled peppers peter piper picked \< /s >
\<s> if peter piper picked a peck of pickled peppers \< /s >
\<s> where s the peck of pickled peppers peter piper picked \</s>

- Compute the vocabulary of the training corpus and print it.    
	- Vocabulary:= ['\<s>', 'peter', 'piper', 'picked', 'a', 'peck', 'of', 'pickled', 'peppers', '\</s>', 'if', 'where', 's', 'the']
	
- In the above training corpus, calculate the probability of each unigram and print the 2 unigrams with
the highest probability. 
	- unigram with highest probability is ' \<s> 'with probability 0.09302325581395349 unigram with second highest Probability ' peter 'with probability 0.09302325581395349
	
- Construct a probability matrix containing the maximum likelihood estimates (MLEs) of all possible bigrams and print it out. 
	- <img width="486" alt="2" src="https://user-images.githubusercontent.com/39759685/133929845-0e98f05d-3839-4381-880b-527f104bfaba.PNG">

- What is the most frequent bigram in this corpus? 
	- <img width="250" alt="3" src="https://user-images.githubusercontent.com/39759685/133929883-8ccad948-fa9c-433b-9bbe-6c93da9bbcaa.PNG">

- Construct a probability matrix containing the Laplace smoothed estimates of all possible bigrams
and print it out. 
	- <img width="497" alt="4" src="https://user-images.githubusercontent.com/39759685/133929905-4c8a6023-98c3-44de-ba0a-99a167d15656.PNG">

- What is the probability of an unseen bigram obtained after using Laplace smoothing? 
	- Check the code
	
- Construct and show a count-of-counts table for the bigrams. 
	- <img width="71" alt="5" src="https://user-images.githubusercontent.com/39759685/133929948-698d8b09-d430-4ff0-ab0f-c52d5086c609.PNG">

9. Briefly explain in your own words the need for smoothing the count-of-counts table. 
10. Consider the following sentence:
\<s> peter piper picked a pickled pepper \</s>
What is the probability of the above test sentence using the following bigram models you created? 
    - MLE bigram model 
    	- 0.0
    - Laplace smoothed bigram model 
    	- 4.317200740854674e-06
