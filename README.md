# Converting Book's Text Into An Audiobook With N Voice Actors

I have done the following sub-tasks using LLMs and "prompt engineering" which won't be trivial at all using traditional NLP tools like SpaCy.

1. Character identification and name clustering (e.g., "Tom", "Tom Sawyer", "Mr. Sawyer", "Thomas Sawyer" -> TOM_SAWYER)
2. Referential gender inference (TOM_SAWYER -> he/him/his)
3. Dialogue attribution or quotation speaker identification with coreference resolution
4. Producing the audio outputs of dialogues by converting Speech Synthesis Markup Language (SSML) input into audio data and finally sticthing them together as one audiobook.

I have used Gemini 1.5 model for the LLM part inspired by GCP's $150 credits and their integrated TTS API.
