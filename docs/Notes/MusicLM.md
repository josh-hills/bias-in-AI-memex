---
Title: MusicLM: Genearting Music From Text
date: 2023-01-31
type: literature
project:
---
tags:: #AI #bias
projects::[[]]

- MusicLM is a machine learning (ML) model that geneartes high-fi music from text descriptions
- Some examples of this that I would be curious to hear: 
	- *A violin melody backed with 808s*
	- *A rock song that only uses humming
	- *90s techno with a strong kick, only using whistling*
- A dataset was release with 5.5k song:text pairs [MusicCaps](https://google-research.github.io/seanet/musiclm/examples/), I love to see researches acting in an open source manner
- This model takes in text (as in the above examples) and outputs up to 5 minutes worth of music, a full song of long-term structure isn't yet solved (maybe this can be done using transformers and tokenization? Just a thought, I'm sure it's been thought of) as it doesn't know how to end
- A big problem for this model is not having enough data, there arent many examples of acoustic scenes annotated with text
- Taking a look at the model, it closely follows the training of [[AudioLM]], the part that makes it different is an additional model that utilizes in the MusicCaps data
- This is a tool that can be used to assist us with creative music tasks

---
### Citational Information

Agostinelli, Andrea, Timo I. Denk, Zalán Borsos, Jesse Engel, Mauro Verzetti, Antoine Caillon, Qingqing Huang, et al. “MusicLM: Generating Music From Text.” arXiv, January 26, 2023. https://doi.org/10.48550/arXiv.2301.11325.


---

### Related Links
- The reality differs a bit from what the professor mentioned in class on [[Jan 30 Lec]]
- MusicLM generates songs but not lyrics, it can't create voices like [[AudioLM]] is capible of
- To compare [[AudioLM]] and MusicLM shortly:
	- AudioLM is capible of generating and predicting speech but can only create piano music
	- MusicLM takes in text as an input whereas AudioLM takes in a few seconds of speech/piano .wav file and continues it
	- We can imagine how much more useful MusicLM would be in the long term, just requesting a song and having it generated for us
*Biases*:
- The risks being that samples will reflect biases in the training data (all models have this bias so it's imporant when generating a dataset that we think about it), so music generation for some cultures is underrepresented