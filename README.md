# CxC Data Hackthon Submission
### By Patrick Yi and Kevin Lee

## Inspiration
This project is based on the University of Waterloo CxC Datathon. The classification of medical transcriptions is a challenging topic introduced in several cases. The construction of a classification model that deals with plain text and NLP strategies is renown for its difficulty and this encouraged us to take on the challenge.

## What it does
The purpose of this machine learning model is to take in transcription data as input and produce a classification of medical specialties written in the transcript. The transcripts are unorganized, plain text information that needs to be cleansed and delivered into a structured and classified form.

## How we built it
The key point we focused in this project was the organization of data before the modeling process could take place. We started with applying basic data cleansing processes such as lower case unification and null value removal. Then, we adopted strategies such as stop word removal, tokenization and assigning POS tags and extracting keywords in nouns. After the data was cleansed and we had structured data consisting only of key words that are meaningful to the classification, we used the distilbert-base-uncased model to train the machine.

## Challenges we ran into
First of all, instead of having a variety in choice of the model, there weren't many options to choose from so we could not leverage and select the 'best model' we could find. Also, based on the fact that we observed numerous overlapping words that possibly could impact the machine learning process, we acknowledged that there is a need to eliminate the effect of this repetitiveness. For instance, words such as 'surgery' or 'patient' were observed more that 1000 times each. However, due to the fact that the test set and the training set consisted of different words/terms, we could not find a justified threshold to remove these unnecessarily repeated words.
## Accomplishments that we're proud of
Using the strategies stated above, we could at least successfully produce a thoroughly cleansed set of data with the keywords we were looking for. Despite this project being our very first ML project in NLP, we could produce a solid conclusion regardless of the significance. 

## What we learned
We believe that we took a step into the NLP realm quite smoothly. We acknowledged which concepts or skills we have to focus on and develop for future projects/opportunities. An example of a concept we are going to look into is the TfidfVectorizer. 

## What's next for Intact : Predict Medical Specialty from Medical Notes
If the classification for the medical notes become more firm, the next steps would be to extract certain categories automatically.