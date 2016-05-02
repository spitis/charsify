### Charisfy

This is a work-in-progress front-end for a tool that allows users to assign labels to different characters of a text. For example, in a two paragraph 5-star review, we might label the first character of each paragraph an `start_paragraph`, the last character of each paragraph an `end_paragraph`, each noun as a `part_of_speech_noun`, all characters except for one caveat the reviewer had as `positive_sentiment` and all characters as `first_person`. Characters will be able to have multiple labels, and there is no restriction on the kinds of labels.

The goal is to create a character-level data set that will be able to classify characters in arbitrary texts. The hope is that after a sufficient amount and variety of labeled examples are available, a trained model will be able to adapt to learn new labels quickly.

The applications for character-level labels are endless:
- Rather than being restricted to classifying entire passages as positive or negative sentiment, we could classify specific sentences or clauses as positive or negative sentiment.
- Once classes are available, we will be able to use this data to do interested text manipulation and parsing. For example, a model trained on certain special sequences of characters could brute force certain parsing tasks for which designing appropriate regular expressions would be painful or outright impossible (e.g., for fake email or phone number recognition). Another trained model could be used to generate the "reverse" of the sentiment of a sentence.
- We could detect and extract parts of interest from large documents (e.g., extracting certain provisions of interest from legal contracts).

### Usage

To run the Charsify front-end, make sure you have a recent version of node installed, clone this repo, run `npm install` followed by `npm start`, and visit localhost:8080 in your browser. 
