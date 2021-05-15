# NLP_TextBlob




NLP using TextBlob python library TextBlob:

TextBlob is a python library and offers a simple API to access its methods and perform basic NLP tasks.

Setting up the System

Installation of TextBlob in your system in a simple task, all you need to do is open anaconda prompt ( or terminal if using Mac OS or Ubuntu) and enter the following commands:

pip install -U textblob

For the uninitiated – practical work in Natural Language Processing typically uses large bodies of linguistic data, or corpora. To download the necessary corpora, you can run the following command:

python -m textblob.download_corpora

NLP tasks using TextBlob:

Tokenization
Tokenization refers to dividing text or a sentence into a sequence of tokens, which roughly correspond to “words”. This is one of the basic tasks of NLP. To do this using TextBlob, follow the two steps:

Create a textblob object and pass a string with it. Call functions of textblob in order to do a specific task.

Noun phrase extraction
Noun Phrase extraction is particularly important when you want to analyze the “who” in a sentence

3.POS-Tagging

Part-of-speech tagging or grammatical tagging is a method to mark words present in a text on the basis of its definition and context. In simple words, it tells whether a word is a noun, or an adjective, or a verb, etc. This is just a complete version of noun phrase extraction, where we want to find all the the parts of speech in a sentence.

Words inflection and lemmatization
Inflection is a process of word formation in which characters are added to the base form of a word to express grammatical meanings. Word inflection in TextBlob is very simple, i.e., the words we tokenized from a textblob can be easily changed into singular or plural. Words can be lemmatized using the lemmatize function.

N-grams
A combination of multiple words together are called N-Grams. N grams (N > 1) are generally more informative as compared to words, and can be used as features for language modelling.
N-grams can be easily accessed in TextBlob using the ngrams function, which returns a tuple of n successive words.

6.Sentiment Analysis

Sentiment analysis is basically the process of determining the attitude or the emotion of the writer, i.e., whether it is positive or negative or neutral.

The sentiment function of textblob returns two properties, polarity, and subjectivity.

Polarity is float which lies in the range of [-1,1] where 1 means positive statement and -1 means a negative statement. Subjective sentences generally refer to personal opinion, emotion or judgment whereas objective refers to factual information. Subjectivity is also a float which lies in the range of [0,1].

Other cool things to do:

Spelling Correction
Spelling correction is a cool feature which TextBlob offers, we can be accessed using the correct function as shown below.

We can also check the list of suggested word and its confidence using the spellcheck function.

2.Creating a short summary of a text

import random

Translation and Language Detection
TextBlob will automatically detect the language and translate into the desired language.

Text classification using TextBlob
first, we need to prepare a training and testing data.

Textblob provides in-build classifiers module to create a custom classifier.

import it and create a basic classifier. TextBlob also offers Decision tree classifier

check the accuracy of this classifier on the testing dataset and also TextBlob provides us to check the most informative features.
