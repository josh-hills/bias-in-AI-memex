---
Title: Word2Vec
date: 2023-02-09
type: literature
project:
---
tags:: #AI #NLP
projects::[[]]

- Word2Vec is a Machine Learning model developed by google
	- While it's developed by google, it isn't a google product and was created for research purposes only
- Important definitions before going more in depth of the model
	- Vector: (short form being vec), for the sake of this paper just imagine this as a number representation for words
- This is a model that takes in a text corpus in as training data and produces word vectors as output
- An example of this is understanding the similarity between words for example:
	- The vector('France') is shown to have a high similarity with vector('Spain') and vector('Belguim')
	- Also, interestingly we can add and subtract vectors and get resulting words:
		- vector('Paris') - vector('France') + vector('Italy') results in vector close to vector('Rome')
			- This indicates the association between Paris and France is similar to the association between Italy and Rome
- Now that we understand what Word2Vec is, we can talk about the dataset used to train the model:
	- The Word2Vec model that google provides is 100 billion words trained on news articles
---
### Citational Information
_Google Code Archive—Long-term storage for Google Code Project Hosting._ (n.d.). July 29, 2013 Retrieved February 9, 2023, from [https://code.google.com/archive/p/word2vec/](https://code.google.com/archive/p/word2vec/)

---

### Related Links

- Because of the nature of this dataset, many biases arise, see [[What biases exist in machine learning models]], and more importantly for this dataset [[Exploring Gender Bias in Word2Vec]]
- Studying these models are increasingly solidifying my view that: Machine Learning models aren't inherintly discriminitory
	- The data that we feed them teaches them exactly what they will become
	- This emphasizes the point that we need to do our best in eliminating biases online (this is typically where we pull data from, which makes sense because it's easily accessable, already digitized information)