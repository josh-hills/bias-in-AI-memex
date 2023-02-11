---
Title: AudioLM: a Language Modeling Approach to Audio Generation
date: 2023-01-31
type: literature
project:
---
tags:: #AI #bias 
projects::[[]]

- This outlines foundational research for the mentioned MusicLM in class [[Jan 30 Lec]]
- Just as speech compines local structures (such as syllables and phonemes) into *words/sentences*, this machine learning (ML) model combines notes into *musical phrases* or songs
- When creating datasets for machine learning models we typically need to figure a way to represent data as text
	- Using speech as an analogy, we need text transcripts to correlate the words someone is saying to text to build speech -> models (this is how siri/google home works)
	- For music we require a textual representation, as example we use MIDI to represent piano music. [See what exactly MIDI is](https://www.britannica.com/art/MIDI-music-technology)
		- MIDI fails in stylistic components, as it only represents notes
- For this case of this model, we don't use MIDI in order to include those stylistic componenets, another ML model is used called wav2vec-BERT, which turns .wav files into vectors (which are used to then train a new model)
- A series of models are trained using these vectors, and finally a model is constructed
- This model is capible of two main things: 
	1. Speech continuation: given a person saying a few words, this model will continue what they are saying. This means it understands the speaker characteristics, [prosody](https://www.britannica.com/art/prosody) and the context of what they're saying
	2. Piano continuation: generates music coherent with the melody, rhythm and harmony of the input
- The speech it generates is hard to distinguish from a real person
- I think it's great that google also generated a model that can detect speech generated with AudioLM, this means it wouldn't be able to be used for a "deep-fake" like effect. 
	- I think it's really important that we fail-proof AI like this

---
### Citational Information

AudioLM: a Language Modeling Approach to Audio Generation (2022). Available at: [[https://ai.googleblog.com/2022/10/audiolm-language-modeling-approach-to.html]] (Accessed: 31 January 2023).


---

### Related Links

- This connects directly with [[Jan 30 Lec]], AudioLM is a less specific (more dumbed down) version of MusicLM
- AudioLM is able to create speech and music
- Studying AudioLM allows us to see the change and improvement that MusicLM provides
- It's amazing to see where the technology of music automation has started and moved toward, as a Computer Scientist I am most interested in the future of technology.
	- Understanding the roots is important to forecasting the future
	- [Ada Lovelace](https://www.britannica.com/biography/Charles-Babbage) comes to mind, manipulating Babbage's machines to compute Bernoulli numbers
		- This technology eventually led to music boxes, and with the technological revololution, synthasizers
- **Biases**:
- There exists bias in this model, as seemingly with most models.
	- There is an under represented variety of accents in voice continuation
		- The accents that exist, at least given examples, are mainly US english speakers
			- By this I mean it performs better on voice continuation of this accent specifically
