# Label sentences in a Japanese sentence Anki deck with the lesson number of Heisig's Remembering the Kanji.

With the Jupyter Notebook in this repository, you will create a new Anki deck with sentence cards that are labeled for the last lesson you would need to have reviewed in Heisig's Remembering the Kanji 1. For instance, if a sentence contains both the kanji characters 十 and 時, lessons 10 and 171 respectively, it would get labeled as 171, since you won't be able to write all characters in that sentence until you have finished that one.

You will need a Python installation to run this notebook. I think it's easiest to just download Anaconda here: https://www.anaconda.com/distribution/ I myself have Python 3.7; I'm not sure this will work in Python 2.x. There are two exeternal libraries needed, but the pip install commands are within the notebook itself.

In addition, you will need to add two decks to your Anki collection. For Heisig's kanji list, I used this deck: https://ankiweb.net/shared/info/1654787298; for the sentences, I used a deck which I sadly can no longer find, but I believe this is a good match: https://ankiweb.net/shared/info/2141233552 In essence, you can use whichever deck you like, but it will require some editing on your part.

The notebook will first open you Anki collection and read in the sentence and kanji cards. I select the sentences with furigana, their translation and the reference to the audio file used; for the kanji, I just select the character and the lesson number. Next I cross-reference them, add the final lesson number to each sentence and create a new deck with the furigana, translation, audio and Heisig number as fields. I then add that deck to my Anki collection. Note that I do not directly edit anything in my Anki collection, as I found the library used was very buggy when it came to saving changes to my collection.

I used this blog post as a reference on how to make a new Anki deck: https://charly-lersteau.com/post/2019-11-17-create-anki-deck-csv/
