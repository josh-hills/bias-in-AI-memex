---
Title: What biases exist in machine learning models
date: 2023-02-09
type: permanent
project:
---

tags::  #bias #AI
projects::[[]]

- I'm curious after doing some readings on [[MusicLM]] and [[AudioLM]]: how was data they have collected and does it avoid biases that could be reflected?
- Before I dig into this, I'll reflect quickly on how I imagine AI (Artificial Intelligence) models reflect biases
	- It really depends on the model but to use the example of NLP (natural language processing):
		- NLP generates text by learning text representations through text data, it builds associations between words to understand how it works
		- Where does bias come in?
			- Well as the professor mentioned in [[Jan 30 Lec]], models reflect the data they were trained on
			- This means if a NLP model is trained on the text of twitter users, it might reflect opinions and associations that twitter users share
			- This can be really dangerous, we can imagine an AI that associates racist, homophobic or misogynistic views
			- For example the AI may create an association between racialized groups and lower income jobs.
				- I can imagine an AI that is given resumes and tries to find the ideal candidate.
					- If the AI is trained on data of the company's past employment, it may reflect similar biases (ex. hiring men more often than women, hiring people with white names and other possibly horrible associations)
	- I think it's super important that when we develop AI models we take a close look at the dataset, making sure we avoid bias
		- This forces me to look at the biases that our society currently reflects 