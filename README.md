# Music Analysis Project
Analyzing Songs using Python and R and using the data to train a RNN/LSTM.

## About
I came up with the idea for this project by looking for a way to combine my interest in music (and the humanities overall) with my desire to create something and using my computational linguisic skills.
The dataset used for this project is the (380,000+ lyrics from MetroLyrics)[https://www.kaggle.com/gyani95/380000-lyrics-from-metrolyrics] Dataset by (Gyandera Mishra)[https://www.kaggle.com/gyani95]. It had a lot of pre-processing to be done but was the largest set of lyrics i could find.s

## Dataset
### Overview 
The dataset is divided into six columns.
1. Index
2. Songname
3. Year
4. Artist
5. Genre
6. Lyrics

### Preparation
Loading the dataset into R Studio helped identify missing or incorrect values. For the sake of simplicity I decided to just remove the songs which had errors in them.
Here's the problems I encountered:
- songs labelled with the year 2038 (which happens to be in the future)
- instrumentals / songs without lyrics (with multiple different labels)
- other languages besides english (again, removed for simplicity's sake)
- broken encodings
- tags such as "\[Verse]"or "\[Chorus]" or “It' Going Down Written by Forch Fabalon Produced by FRE$H488! Running Time: 3:02 (INTRO)” 
- size (At the time of this project the laptop i used didn't have a lot of processing power)
